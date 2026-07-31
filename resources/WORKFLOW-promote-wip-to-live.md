# Workflow — promoting a repo from **In Progress** to the **Knowledge Base** grid

Follow this when a repo that currently renders as a grey gradient WIP card has shipped its GitHub
Pages site and is ready to appear as a coloured, clickable card with an in-page chapter index.

Everything lives in a single file: [index.html](../index.html). There is no build step — edit,
commit, push, done.

---

## 0. Preconditions — do not promote until all three are true

| Check | How |
|---|---|
| The Pages site is live | Open `https://karam-nus.github.io/<repo>/` — it must render, not 404 |
| Chapters are reachable | Open two or three chapter URLs directly, e.g. `.../<repo>/03_something` |
| GitHub Pages is enabled on the right branch | Repo → Settings → Pages → *Source* points at the branch/folder that holds the content |

A repo with a published index page but broken chapter links should stay in the WIP section.

---

## 1. Where things live in `index.html`

Page order, for orientation: **top bar → "Let's Learn!" hero → Knowledge Base grid → In Progress
grid → About → footer.** A promotion moves a card from the third block to the second; the hero and
the About paragraph are static and need no edits.

All page content is driven by one array near the top of the `<script>` block:

```js
const repos = [
  {
    id:      'vision',                                   // slug — also the URL hash (#vision)
    label:   'VISION',                                   // big text on the card
    blurb:   'Pixels to predictions — CV tasks, …',      // one-liner under the title
    color:   'mint',                                     // palette token (see PALETTE below)
    status:  'live',                                     // 'live' | 'wip'  ← the switch
    url:     'https://karam-nus.github.io/vision/',      // where the → arrow goes
    base:    'https://karam-nus.github.io/vision/',      // prefix for every chapter link
    groups: [
      { name:'Foundations', chs:[
        { n:'01', t:'Image Fundamentals', u:'01_image_fundamentals', d:'images as tensors' },
        { n:'02', t:'Not written yet',    u:null,                    d:'planned' },
      ]},
    ],
  },
  …
]
```

Rendering is driven entirely off `status`:

- `status: 'live'` → coloured card, clickable, arrow link, expandable chapter index.
- `status: 'wip'` → plain grey card on the shared gradient banner, no arrow, not focusable,
  `groups` ignored.

There is no scope-badge field. The badge (`42 chapters`) is counted from `groups` — or from
`pillGroups` for `metrics` — at render time, so it cannot drift from the actual index.

A chapter with `u: null` renders dim and non-clickable — use it for chapters you have planned but
not yet written inside an otherwise-live repo.

---

## 2. The promotion, step by step

### Step 1 — branch

```bash
cd ~/work/personal/github/karam-nus.github.io
git switch main && git pull
git switch -c promote-<repo>
```

### Step 2 — find the WIP entry

Search `index.html` for the repo's `id`. It will look like:

```js
{ id:'quantization', label:'QUANTIZATION',
  blurb:'PTQ, QAT and the full quantization landscape',
  status:'wip' },
```

### Step 3 — build the chapter index

Get the real chapter list from the source repo rather than typing it from memory:

```bash
ls ../quantization/*.md            # or docs/, or _chapters/ — match the repo's layout
head -3 ../quantization/*.md       # front-matter titles
```

The chapter URL slug is the filename without `.md` (Jekyll on Pages strips the extension), so
`03_calibration.md` → `u: '03_calibration'`. Confirm one in the browser before doing all of them.

### Step 4 — rewrite the entry

Flip `status`, then add the three fields a live card needs — `color`, `url`, `base` — plus
the `groups` array:

```js
{
  id:     'quantization',
  label:  'QUANTIZATION',
  blurb:  'PTQ, QAT and the full quantization landscape',
  color:  'sand',                                           // ← see PALETTE
  status: 'live',                                           // ← was 'wip'
  url:    'https://karam-nus.github.io/quantization/',
  base:   'https://karam-nus.github.io/quantization/',
  groups: [
    { name:'Foundations', chs:[
      { n:'01', t:'Why Quantize', u:'01_why_quantize', d:'memory, bandwidth, latency' },
      …
    ]},
  ],
}
```

Then **move the object** out of the WIP block and into the live block, in the position you want it
to appear on the grid. Order in the array *is* order on the page.

### Step 5 — pick the colour

See PALETTE below. Two rules only:

1. Never place two cards of the same colour side by side or directly above/below each other.
2. Keep roughly one `ink` card per visual row — that near-black block is what gives the grid its
   rhythm. If promoting a repo pushes the `ink` card into a bad spot, reassign colours across the
   whole grid; it takes thirty seconds and matters more than which repo gets which hue.

### Step 6 — verify locally

```bash
python3 -m http.server 8000        # then open http://localhost:8000
```

Walk this checklist:

- [ ] Card appears in the Knowledge Base grid, not the In Progress grid.
- [ ] The hero sub-line count went up by one on its own. It is derived from
      `repos.filter(r => r.status === 'live').length` — if it's stale, someone hard-coded a number;
      fix that rather than editing the text.
- [ ] Colour does not clash with its neighbours; the row rhythm still reads.
- [ ] Clicking the card body expands the chapter index inline, below that card's row.
- [ ] Clicking the `→` opens the live site in a **new tab** and does *not* toggle the panel.
- [ ] Every chapter link in the expanded panel opens a real page (spot-check first, middle, last).
- [ ] Scope badge matches the actual chapter count. It is derived, so a wrong number means the
      `groups` array is wrong — fix the data, not the badge.
- [ ] Toggle light/dark — text is legible on the card in both.
- [ ] Narrow the window to phone width — grid reflows, panel still lands below the right row.
- [ ] Browser console is clean.

Fast link check from the terminal:

```bash
grep -o "https://karam-nus.github.io/quantization/[a-z0-9_]*" index.html \
  | sort -u \
  | xargs -I{} sh -c 'printf "%s " {}; curl -s -o /dev/null -w "%{http_code}\n" {}'
```

Anything that isn't `200` is either a wrong slug or a chapter that should be `u: null`.

### Step 7 — keep `README.md` in step

The repo README mirrors the same index as a `<details>` block. Add or update the matching section
so GitHub and the Pages site don't drift apart.

### Step 8 — ship

```bash
git add index.html README.md
git commit -m "promote quantization from WIP to live knowledge base"
git push -u origin promote-<repo>
```

Open a PR, or merge to `main` directly if you're working solo. Pages redeploys via
`.github/workflows/deploy-pages.yml`; give it a minute, then hard-reload
`https://karam-nus.github.io/karam-nus/` and confirm the card is there.

---

## PALETTE

Live cards (`color` token → surface / text):

| Token | Surface | Text |
|---|---|---|
| `mint` | `#C3E8C9` | `#0F1A11` |
| `sky` | `#B8E4F0` | `#0C1A1F` |
| `ink` | `#0E0E0E` | `#F5F5F5` |
| `peach` | `#F6CFB2` | `#20140A` |
| `salmon` | `#F3BCAF` | `#21100C` |
| `sand` | `#EDD9AE` | `#1E1808` |
| `pink` | `#F6BFE9` | `#20101C` |
| `periwinkle` | `#C9C6F9` | `#12102A` |

WIP cards take no `color`. They are plain grey (`.card-wip`) sitting on the shared gradient banner
(`.wip-banner`), which is defined once in CSS. Nothing to choose, nothing to maintain.

---

## Going the other way (live → WIP)

Rare, but if a repo's Pages site breaks or gets gutted: set `status: 'wip'`, delete
`color`, `url`, `base` and `groups`, and move the object down into the WIP block. Keep `id`,
`label` and `blurb`. The chapter data is recoverable from git history if you need it back.

---

## Adding a brand-new repo

Same as a promotion, minus Step 2. Append a new object to `repos[]` — `status: 'wip'` if it's just
a README stub, `status: 'live'` with a full `groups` array if it shipped complete. Everything else
(card, grid position, expansion panel, hash link) is generated from that one object.
