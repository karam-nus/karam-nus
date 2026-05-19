<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:000000,100:000000&height=180&section=header&text=Karamjot%20Singh&fontSize=48&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=AI+Research+Scientist+%C2%B7+Model+Optimization+%C2%B7+NUS+Singapore&descSize=15&descAlignY=62&descColor=555555" width="100%" />

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=2800&pause=900&color=FFFFFF&center=true&vCenter=true&width=700&height=45&lines=Quantization+%C2%B7+AWQ+%C2%B7+GPTQ+%C2%B7+SmoothQuant;HPC+Inference+%C2%B7+vLLM+%C2%B7+TensorRT-LLM;LLM+Architecture+%C2%B7+Agents+%C2%B7+Evals;Model+Optimization+Researcher+%40+NUS)](https://git.io/typing-svg)

</div>

---

AI Research Scientist · Model Optimization · **NUS Singapore** · [🤗 karamjotsingh](https://huggingface.co/karamjotsingh)

---

## Knowledge Base

<details>
<summary><kbd>LANGUAGE MODELLING</kbd> &nbsp;·&nbsp; 38 chapters + 3 appendices &nbsp;<a href="https://karam-nus.github.io/language-modelling/">↗</a></summary>
<br>

**Foundations**

`01` [Introduction to Language Modelling](https://karam-nus.github.io/language-modelling/01_introduction) · text → tokens → tensors → predictions  
`02` [Embeddings & Representations](https://karam-nus.github.io/language-modelling/02_embeddings) · dense vectors, RoPE, ALiBi, geometry of meaning  
`03` [The Transformer](https://karam-nus.github.io/language-modelling/03_the_transformer) · complete architecture walkthrough with tensor shapes  
`04` [Attention — SDPA & Multi-Head](https://karam-nus.github.io/language-modelling/04_attention_sdpa_and_mha) · Q/K/V math, causal masking, Flash Attention

**Attention & Architecture**

`05` [Attention Variants — GQA, MQA & MLA](https://karam-nus.github.io/language-modelling/05_attention_gqa_mqa_mla) · KV bottleneck, sliding window, tensor shape comparisons  
`06` [Decoder-Only Models](https://karam-nus.github.io/language-modelling/06_decoder_only_models) · GPT family, LLaMA architecture, open-source landscape  
`07` [Encoder & Seq2Seq Models](https://karam-nus.github.io/language-modelling/07_encoder_and_seq2seq_models) · BERT, T5, BART — encoder vs decoder vs encoder-decoder  
`08` [Multimodal Models](https://karam-nus.github.io/language-modelling/08_multimodal_models) · ViT, Whisper, modality fusion, image-to-token pipelines

**Training**

`09` [Data for LLMs & VLMs](https://karam-nus.github.io/language-modelling/09_data_for_llms) · pre-training, SFT, RLHF, RL data formats & tensor shapes  
`10` [Pre-Training at Scale](https://karam-nus.github.io/language-modelling/10_pretraining_at_scale) · data curation, training objectives, loss curves  
`11` [Optimizers & Loss Functions](https://karam-nus.github.io/language-modelling/11_optimizers_and_loss_functions) · AdamW, Adam-mini, Muon, SOAP, DPO loss  
`12` [Mid-Training & Continued Pre-Training](https://karam-nus.github.io/language-modelling/12_mid_training) · long-context extension, domain adaptation, annealing  
`13` [Fine-Tuning & Adaptation](https://karam-nus.github.io/language-modelling/13_finetuning_and_adaptation) · SFT, LoRA, QLoRA  
`14` [PEFT: LoRA, QLoRA & Variants](https://karam-nus.github.io/language-modelling/14_peft_lora_and_variants) · rank decomposition math, DoRA, rsLoRA, VeRA  
`15` [Alignment — RLHF & Beyond](https://karam-nus.github.io/language-modelling/15_alignment_rlhf_and_beyond) · reward models, PPO, DPO, Constitutional AI

**Inference & Generation**

`16` [Inference & Sampling Strategies](https://karam-nus.github.io/language-modelling/16_inference_and_sampling) · temperature, top-k/p, speculative decoding, structured output  
`17` [KV-Cache — Mechanics & Memory](https://karam-nus.github.io/language-modelling/17_kv_cache_mechanics) · tensor shapes through generation, memory calculations  
`18` [KV-Cache — Optimization Strategies](https://karam-nus.github.io/language-modelling/18_kv_cache_optimization) · PagedAttention, continuous batching, KV quantization

**Quantization**

`19` [Data Types & Numerical Precision](https://karam-nus.github.io/language-modelling/19_data_types_and_precision) · FP32 → FP4 bit layouts, BF16 vs FP16  
`20` [Quantization Fundamentals](https://karam-nus.github.io/language-modelling/20_quantization_fundamentals) · affine math, calibration, weight-only vs W+A  
`21` [Quantization Techniques — Full Landscape](https://karam-nus.github.io/language-modelling/21_quantization_techniques) · GPTQ, AWQ, SmoothQuant, KIVI, BitNet  
`22` [Quantization Benchmarks & Selection](https://karam-nus.github.io/language-modelling/22_quantization_benchmarks) · perplexity vs bits, throughput, GGUF guide  
`23` [Knowledge Distillation & QAD](https://karam-nus.github.io/language-modelling/23_knowledge_distillation) · feature distillation, fake quantization with STE

**Hardware & Kernels**

`24` [GPU Architecture for ML](https://karam-nus.github.io/language-modelling/24_gpu_architecture) · SMs, Tensor Cores, roofline model, A100/H100/B200  
`25` [CUDA & Kernel Development](https://karam-nus.github.io/language-modelling/25_cuda_and_kernel_development) · Triton kernels, Flash Attention design, fused ops  
`26` [Distributed Training](https://karam-nus.github.io/language-modelling/26_distributed_training) · DDP, FSDP, DeepSpeed ZeRO, 3D parallelism  
`27` [ASICs & Specialized Accelerators](https://karam-nus.github.io/language-modelling/27_asics_and_accelerators) · TPUs, Groq, Trainium, Apple Silicon

**Ecosystem & Tooling**

`28` [The Hugging Face Ecosystem](https://karam-nus.github.io/language-modelling/28_huggingface_ecosystem) · Hub, Spaces, datasets, tokenizers  
`29` [Transformers Library Deep Dive](https://karam-nus.github.io/language-modelling/29_transformers_library) · AutoModel, Trainer, Pipeline internals  
`30` [Evaluation & Benchmarks](https://karam-nus.github.io/language-modelling/30_evaluation_and_benchmarks) · MMLU, HumanEval, lm-eval-harness  
`31` [Serving & Deployment](https://karam-nus.github.io/language-modelling/31_serving_and_deployment) · vLLM, TGI, TensorRT-LLM, Ollama

**Advanced Topics**

`32` [Scaling Laws & Emergent Abilities](https://karam-nus.github.io/language-modelling/32_scaling_laws) · Kaplan, Chinchilla, emergence debate  
`33` [Mixture of Experts](https://karam-nus.github.io/language-modelling/33_mixture_of_experts) · sparse routing, Mixtral, DeepSeek-MoE  
`34` [SSMs & Beyond Transformers](https://karam-nus.github.io/language-modelling/34_ssms_and_alternatives) · Mamba, RWKV, Jamba  
`35` [Reasoning Models](https://karam-nus.github.io/language-modelling/35_reasoning_models) · chain-of-thought, o1-style, test-time compute  
`36` [Retrieval-Augmented Generation](https://karam-nus.github.io/language-modelling/36_rag) · RAG pipeline, vector databases, advanced retrieval  
`37` [Agents & Tool Use](https://karam-nus.github.io/language-modelling/37_agents_and_tool_use) · function calling, coding agents, MCP protocol  
`38` [The Frontier](https://karam-nus.github.io/language-modelling/38_frontier) · long context, world models, interpretability

**Appendices**

`A` [History of Language Modelling](https://karam-nus.github.io/language-modelling/appendix_a_history) · Shannon → GPT-4  
`B` [Tokenization Deep Dive](https://karam-nus.github.io/language-modelling/appendix_b_tokenization) · BPE, WordPiece, SentencePiece  
`C` [HuggingFace Config Reference](https://karam-nus.github.io/language-modelling/appendix_c_model_config) · every config.json parameter explained

</details>

---

<details>
<summary><kbd>MODELS</kbd> &nbsp;·&nbsp; 7 architecture families &nbsp;<a href="https://karam-nus.github.io/models/">↗</a></summary>
<br>

Architecture deep-dives across generations — release timelines, benchmark tables, HTML diagrams, 10-point version summaries, community perspectives.

`01` [Qwen](https://karam-nus.github.io/models/01_Qwen) · v1 → 1.5 → 2 → 2.5 → 3  
`02` [Llama](https://karam-nus.github.io/models/02_Llama) · v1 → 2 → 3 → 3.1 → 3.2 → 3.3 → 4  
`03` DeepSeek · V1 → V2 → V3 → R1 *(planned)*  
`04` [Gemma](https://karam-nus.github.io/models/04_Gemma) · v1 → 2 → 3 → 4  
`05` Mistral · 7B → Mixtral → Large *(planned)*  
`06` Phi · v1 → 1.5 → 2 → 3 → 4 *(planned)*  
`07` [Alpamayo](https://karam-nus.github.io/models/07_Alpamayo) · R1 → 1.5 (VLA)

</details>

---

<details>
<summary><kbd>INFERENCE</kbd> &nbsp;·&nbsp; 12 chapters &nbsp;<a href="https://karam-nus.github.io/inference/">↗</a></summary>
<br>

From quantized model to production — the complete deployment guide for AI research scientists.

`01` [Grand Overview](https://karam-nus.github.io/inference/01_grand_overview) · full stack: PyTorch model → hardware execution  
`02` [Glossary & Concept Map](https://karam-nus.github.io/inference/02_glossary_and_concept_map) · every term defined + visual relationship maps  
`03` [Inference Engines Deep Dive](https://karam-nus.github.io/inference/03_inference_engines) · vLLM, SGLang, llama.cpp, TensorRT-LLM — compared  
`04` [Runtimes & Backends](https://karam-nus.github.io/inference/04_runtimes_and_backends) · ONNX Runtime, CUDA, ROCm, OpenVINO, ExecuTorch  
`05` [Hardware Landscape](https://karam-nus.github.io/inference/05_hardware_landscape) · NVIDIA, AMD, Intel, TPUs, NPUs, custom ASICs  
`06` [Quantization to Deployment Bridge](https://karam-nus.github.io/inference/06_quantization_to_deployment) · how your quantized model gets deployed end-to-end  
`07` [Company Landscape](https://karam-nus.github.io/inference/07_company_landscape) · NVIDIA, Renesas, Synopsys, Qualcomm  
`08` [Model Formats & Serialization](https://karam-nus.github.io/inference/08_model_formats) · GGUF, ONNX, SafeTensors, TorchScript  
`09` [Serving Infrastructure & Middleware](https://karam-nus.github.io/inference/09_serving_and_middleware) · Triton, KServe, API gateways, load balancers  
`10` [Edge & Embedded Deployment](https://karam-nus.github.io/inference/10_edge_and_embedded) · TFLite, ExecuTorch, microcontrollers, Renesas MCUs  
`11` [Compiler Stack](https://karam-nus.github.io/inference/11_compiler_stack) · TVM, XLA, Triton compiler, MLIR  
`12` [Practical Code Guide](https://karam-nus.github.io/inference/12_practical_code_guide) · PyTorch → quantize → export → deploy → serve

</details>

---

<details>
<summary><kbd>AGENTS</kbd> &nbsp;·&nbsp; 14 chapters &nbsp;<a href="https://karam-nus.github.io/agents/">↗</a></summary>
<br>

From zero to agent developer — understanding, building, and deploying AI agents & agentic workflows.

**Foundation**

`01` [What Are Agents?](https://karam-nus.github.io/agents/01_what_are_agents) · definition, paradigm shift from LLMs, when to use agents  
`02` [History & Evolution](https://karam-nus.github.io/agents/02_history_and_evolution) · ELIZA → expert systems → ReAct → autonomous agents  
`03` [Anatomy of an Agent](https://karam-nus.github.io/agents/03_anatomy_of_an_agent) · the 4 pillars: LLM brain, tools, memory, planning  
`04` [The Agent Loop](https://karam-nus.github.io/agents/04_the_agent_loop) · observe → think → act cycle, autonomous execution

**Core Capabilities**

`05` [Tools & Function Calling](https://karam-nus.github.io/agents/05_tools_and_function_calling) · function calling APIs, MCP protocol, custom tools  
`06` [Memory Systems](https://karam-nus.github.io/agents/06_memory_systems) · working memory, short/long-term, vector stores, RAG  
`07` [Planning & Reasoning](https://karam-nus.github.io/agents/07_planning_and_reasoning) · CoT, ReAct, Reflexion, task decomposition

**Scaling Up**

`08` [Multi-Agent Systems](https://karam-nus.github.io/agents/08_multi_agent_systems) · communication patterns, supervisor & swarm architectures  
`09` [Agentic Frameworks & SDKs](https://karam-nus.github.io/agents/09_agentic_frameworks) · LangGraph, CrewAI, AutoGen, OpenAI Agents SDK

**Hands-On & Production**

`10` [Build Your First Agent](https://karam-nus.github.io/agents/10_build_your_first_agent) · research assistant with OpenAI SDK + LangGraph  
`11` [Agentic Design Patterns](https://karam-nus.github.io/agents/11_agentic_design_patterns) · router, orchestrator-worker, evaluator-optimizer, HITL  
`12` [Deployment & Production](https://karam-nus.github.io/agents/12_deployment_and_production) · observability, cost management, safety guardrails  
`13` [Open Source Landscape](https://karam-nus.github.io/agents/13_open_source_landscape) · 30+ curated projects: frameworks, apps, benchmarks, infra  
`14` [Career Guide](https://karam-nus.github.io/agents/14_career_guide) · skills roadmap, portfolio projects, interview topics

</details>

---

<details>
<summary><kbd>NVIDIA</kbd> &nbsp;·&nbsp; 13 chapters + 2 appendices &nbsp;<a href="https://karam-nus.github.io/nvidia/">↗</a></summary>
<br>

From silicon to supercomputers — GPU architecture, CUDA, data centers, and the accelerated computing ecosystem.

**Foundations**

`01` [GPU Fundamentals](https://karam-nus.github.io/nvidia/01_gpu_fundamentals) · CPU vs GPU, data types, memory hierarchy, roofline model  
`02` [GPU Microarchitecture](https://karam-nus.github.io/nvidia/02_gpu_microarchitecture) · Streaming Multiprocessors, Tensor Cores, warp execution  
`03` [CUDA Programming](https://karam-nus.github.io/nvidia/03_cuda_programming) · kernels, memory management, streams, Python bindings

**Software Stack**

`04` [NVIDIA Libraries](https://karam-nus.github.io/nvidia/04_nvidia_libraries) · cuBLAS, cuDNN, NCCL, CUTLASS, cuSPARSE  
`05` [Optimization Stack](https://karam-nus.github.io/nvidia/05_optimization_stack) · TensorRT, TensorRT-LLM, ModelOpt, Triton Inference Server  
`06` [NVIDIA Models](https://karam-nus.github.io/nvidia/06_nvidia_models) · Nemotron, Alpamayo, NeMo, ASR/TTS, NIM microservices

**Scaling**

`07` [Parallelism on GPUs](https://karam-nus.github.io/nvidia/07_parallelism) · data, tensor, pipeline, sequence, expert parallelism, ZeRO  
`08` [GPU Generations](https://karam-nus.github.io/nvidia/08_gpu_generations) · GeForce 30→50, H100, H200, B200 — features & VRAM  
`09` [NVIDIA CPUs](https://karam-nus.github.io/nvidia/09_nvidia_cpus) · Grace CPU, Grace Hopper Superchip, ARM in the data center

**Infrastructure & Economics**

`10` [Multi-GPU Interconnects](https://karam-nus.github.io/nvidia/10_multi_gpu_interconnects) · NVLink, NVSwitch, PCIe, InfiniBand  
`11` [Data Center Architectures](https://karam-nus.github.io/nvidia/11_data_center_architectures) · DGX, HGX, SuperPOD, DGX Cloud, full rack design  
`12` [GPU Economics & Tokenomics](https://karam-nus.github.io/nvidia/12_gpu_economics) · cost per token, TCO, cloud vs on-prem  
`13` [ASICs & GPU Competitors](https://karam-nus.github.io/nvidia/13_asics_and_competitors) · Cerebras, Groq, Google TPU, Intel Gaudi

**Appendices**

`A` [Company History & Timeline](https://karam-nus.github.io/nvidia/appendix_a_company_history) · from a Denny's booth (1993) to $3T  
`B` [Future Roadmap](https://karam-nus.github.io/nvidia/appendix_b_future_roadmap) · Rubin, Vera, photonic interconnects, quantum

</details>

---

<details>
<summary><kbd>VISION</kbd> &nbsp;·&nbsp; 42 chapters + 3 appendices &nbsp;<a href="https://karam-nus.github.io/vision/">↗</a></summary>
<br>

From pixels to predictions — CV use cases, architectures, optimization, deployment, and the research frontier.

**Overview & Foundations**

`00` [Grand Overview](https://karam-nus.github.io/vision/00_grand_overview) · full CV landscape — tasks, history, benchmarks  
`01` [Image Fundamentals](https://karam-nus.github.io/vision/01_image_fundamentals) · images as tensors `[B,C,H,W]`, color spaces, preprocessing

**Use Cases**

`02` [Image Classification](https://karam-nus.github.io/vision/02_image_classification) · softmax, zero-shot, ImageNet  
`03` [Object Detection](https://karam-nus.github.io/vision/03_object_detection) · two-stage vs one-stage, NMS deep dive, mAP  
`04` [Semantic Segmentation](https://karam-nus.github.io/vision/04_semantic_segmentation) · encoder-decoder, dilated convolutions, mIoU  
`05` [Instance Segmentation](https://karam-nus.github.io/vision/05_instance_segmentation) · Mask R-CNN, SAM, query-based methods  
`06` [Object Tracking](https://karam-nus.github.io/vision/06_object_tracking) · Kalman filter, Hungarian algorithm, SORT → ByteTrack  
`07` [Pose Estimation](https://karam-nus.github.io/vision/07_pose_estimation) · keypoints, heatmaps, PAF, top-down vs bottom-up  
`08` [Face Recognition](https://karam-nus.github.io/vision/08_face_recognition) · detection, alignment, ArcFace/CosFace/SphereFace  
`09` [Depth Estimation](https://karam-nus.github.io/vision/09_depth_estimation) · stereo, monocular depth, LiDAR fusion  
`10` [Optical Flow](https://karam-nus.github.io/vision/10_optical_flow) · Lucas-Kanade, FlowNet, RAFT  
`11` [Video Understanding](https://karam-nus.github.io/vision/11_video_understanding) · action recognition, 3D conv, temporal transformers  
`12` [3D Vision](https://karam-nus.github.io/vision/12_3d_vision) · point clouds, NeRF, 3D Gaussian splatting, SLAM  
`13` [Anomaly Detection](https://karam-nus.github.io/vision/13_anomaly_detection) · one-class learning, PatchCore, reconstruction-based  
`14` [OCR & Document Understanding](https://karam-nus.github.io/vision/14_ocr_and_document_understanding) · CRNN+CTC, LayoutLM  
`15` [Medical Imaging](https://karam-nus.github.io/vision/15_medical_imaging) · segmentation, classification, MedSAM  
`16` [Multimodal Vision Tasks](https://karam-nus.github.io/vision/16_multimodal_vision_tasks) · VQA, captioning, text-to-image

**Architectures**

`17` [CNN Fundamentals](https://karam-nus.github.io/vision/17_cnn_fundamentals) · convolution math, receptive fields, depthwise convs  
`18` [Classification Architectures](https://karam-nus.github.io/vision/18_classification_architectures) · ResNet, MobileNet, EfficientNet, ViT, Swin, ConvNeXt  
`19` [Detection Architectures](https://karam-nus.github.io/vision/19_detection_architectures) · YOLO v1→v11, Faster R-CNN, DETR, RT-DETR  
`20` [Segmentation Architectures](https://karam-nus.github.io/vision/20_segmentation_architectures) · FCN, U-Net, DeepLab v3+, Mask2Former, SAM  
`21` [Pose Architectures](https://karam-nus.github.io/vision/21_pose_architectures) · HRNet, ViTPose, OpenPose, WholeBody  
`22` [Face Architectures](https://karam-nus.github.io/vision/22_face_architectures) · MTCNN, RetinaFace, MobileFaceNet, ArcFace  
`23` [Tracking Architectures](https://karam-nus.github.io/vision/23_tracking_architectures) · SORT, DeepSORT, ByteTrack, StrongSORT  
`24` [Vision Transformers](https://karam-nus.github.io/vision/24_vision_transformers) · ViT, DeiT, Swin, MAE, DINO, DINOv2  
`25` [Multimodal Architectures](https://karam-nus.github.io/vision/25_multimodal_architectures) · CLIP, BLIP-2, LLaVA, Grounding DINO, SAM 2

**Optimization**

`26` [Optimization Overview](https://karam-nus.github.io/vision/26_optimization_overview) · accuracy-speed-size triangle, profiling taxonomy  
`27` [Quantization](https://karam-nus.github.io/vision/27_quantization) · PTQ, QAT, INT8/FP8, mixed precision  
`28` [Pruning & Sparsification](https://karam-nus.github.io/vision/28_pruning_and_sparsification) · structured/unstructured, lottery ticket, ASP  
`29` [Knowledge Distillation](https://karam-nus.github.io/vision/29_knowledge_distillation) · feature mimicking, attention transfer  
`30` [Neural Architecture Search](https://karam-nus.github.io/vision/30_neural_architecture_search) · DARTS, Once-for-All, EfficientNet  
`31` [Efficient Inference](https://karam-nus.github.io/vision/31_efficient_inference) · ONNX, TensorRT, OpenVINO, TFLite, CoreML

**Data & Training**

`32` [Datasets](https://karam-nus.github.io/vision/32_datasets) · ImageNet, COCO, ADE20K, LFW, Kinetics, KITTI, MVTec  
`33` [Data Augmentation](https://karam-nus.github.io/vision/33_data_augmentation) · MixUp, CutMix, Mosaic, AutoAugment, Copy-Paste  
`34` [Training Recipes](https://karam-nus.github.io/vision/34_training_recipes) · loss functions, AdamW, LR schedules, EMA  
`35` [Self-Supervised Learning](https://karam-nus.github.io/vision/35_self_supervised_learning) · SimCLR, MoCo, BYOL, MAE, DINO

**Deployment & Ecosystem**

`36` [Deployment](https://karam-nus.github.io/vision/36_deployment) · ONNX export, Triton/TorchServe, edge (Jetson/mobile)  
`37` [Ecosystem & Libraries](https://karam-nus.github.io/vision/37_ecosystem_and_libraries) · timm, MMDetection, Detectron2, Ultralytics, Roboflow  
`38` [Evaluation & Benchmarks](https://karam-nus.github.io/vision/38_evaluation_and_benchmarks) · mAP computation, OKS, HOTA, FID, Rank-1

**Frontier**

`39` [Vision–Language Models](https://karam-nus.github.io/vision/39_vision_language_models) · CLIP ecosystem, GPT-4V, Gemini Vision  
`40` [Foundation Models](https://karam-nus.github.io/vision/40_foundation_models) · SAM, DINOv2, Florence-2, InternVL  
`41` [Generative Vision](https://karam-nus.github.io/vision/41_generative_vision) · GANs, VAEs, DDPM, Stable Diffusion, ControlNet  
`42` [The Frontier](https://karam-nus.github.io/vision/42_frontier) · world models, 3DGS, embodied AI, neuromorphic vision

**Appendices**

`A` [History of Computer Vision](https://karam-nus.github.io/vision/appendix_a_history) · Hubel & Wiesel → SAM 2  
`B` [Math Foundations](https://karam-nus.github.io/vision/appendix_b_math_foundations) · linear algebra, convolutions, Fourier, probability  
`C` [Glossary](https://karam-nus.github.io/vision/appendix_c_glossary) · every key term, acronym, and metric

</details>

---

<details>
<summary><kbd>EVALS</kbd> &nbsp;·&nbsp; 4 benchmarks &nbsp;<a href="https://karam-nus.github.io/evals/">↗</a></summary>
<br>

From perplexity to multimodal — the math, datasets, code, caveats, and practical wisdom for every major LLM/VLM benchmark.

`01` [Wikitext Perplexity](https://karam-nus.github.io/evals/01_wikitext_perplexity) · language modelling quality, training progress, regression detection  
`02` [MMLU](https://karam-nus.github.io/evals/02_mmlu) · broad academic knowledge across 57 subjects  
`03` [MMMU](https://karam-nus.github.io/evals/03_mmmu) · college-level multimodal understanding across 30 subjects  
`04` [RealWorldQA](https://karam-nus.github.io/evals/04_realworldqa) · real-world spatial and visual understanding from photos

</details>

---

<details>
<summary><kbd>METRICS</kbd> &nbsp;·&nbsp; 58 metrics across 8 domains &nbsp;<a href="https://karam-nus.github.io/metrics/">↗</a></summary>
<br>

Debug model internals. Select the right metric. Understand what each metric reveals — and where it breaks.

**Tensor Comparison & Numerical Debugging** · `cosine similarity` `RMSE` `RRMSE` `MAE` `torch.allclose` `SNR` `SQNR` `KL Divergence` `L1/L2 Norm Diff` `Max Absolute Error` `Pearson/Spearman`

**General Regression** · `MSE` `RMSE` `MAE` `MAPE` `R²` `Huber Loss` `SMAPE`

**Classification** · `Accuracy` `Precision` `Recall` `F1` `ROC-AUC` `PR-AUC` `MCC` `Cohen's Kappa` `Specificity` `Top-K Accuracy`

**Object Detection** · `mAP` `IoU` `GIoU` `DIoU` `CIoU` `Average Recall`

**Segmentation** · `Dice` `IoU (Jaccard)` `Pixel Accuracy` `Boundary F1`

**Generative & Distribution Quality** · `FID` `Inception Score` `LPIPS` `SSIM` `PSNR` `BLEU` `ROUGE` `METEOR` `CIDEr` `BERTScore`

**Ranking & Retrieval** · `NDCG` `MRR` `Precision@K` `Recall@K` `MAP@K`

**Calibration & Uncertainty** · `ECE` `MCE` `Reliability Diagrams` `Brier Score` `NLL`

</details>

---

<details>
<summary><kbd>SOFTWARE ENGINEERING</kbd> &nbsp;·&nbsp; 20 chapters + 3 appendices &nbsp;<a href="https://karam-nus.github.io/software/">↗</a></summary>
<br>

From scripts to production — industry-standard software engineering for ML practitioners.

**Foundations**

`01` [Software Development Lifecycle](https://karam-nus.github.io/software/01_software_development_lifecycle) · Agile & Scrum for ML teams, sprint planning  
`02` [Version Control with Git](https://karam-nus.github.io/software/02_version_control_with_git) · branching strategies, conventional commits, monorepos  
`03` [Code Quality & Style](https://karam-nus.github.io/software/03_code_quality_and_style) · Ruff, Black, mypy, PEP 8, pre-commit hooks  
`04` [Testing for ML Software](https://karam-nus.github.io/software/04_testing_for_ml_software) · pytest, property-based testing, ML-specific patterns  
`05` [Design Patterns](https://karam-nus.github.io/software/05_design_patterns) · Strategy, Factory, Observer, Registry, Pipeline — applied to ML

**Architecture & Design**

`06` [OOP & Functional Design](https://karam-nus.github.io/software/06_oop_and_functional_design) · SOLID, composition vs inheritance, Pydantic  
`07` [API Design & REST](https://karam-nus.github.io/software/07_api_design_and_rest) · FastAPI for model serving, gRPC, versioning  
`08` [Documentation](https://karam-nus.github.io/software/08_documentation) · Sphinx/MkDocs, docstrings, ADRs, README-driven dev  
`09` [Dependency & Package Management](https://karam-nus.github.io/software/09_dependency_and_package_management) · pip, conda, uv, lock files  
`10` [Build Systems & Automation](https://karam-nus.github.io/software/10_build_systems_and_automation) · Makefiles, CI/CD with GitHub Actions

**Infrastructure & Operations**

`11` [Containerization & Reproducibility](https://karam-nus.github.io/software/11_containerization_and_reproducibility) · Docker, multi-stage builds, NVIDIA container toolkit  
`12` [Configuration Management](https://karam-nus.github.io/software/12_configuration_management) · Hydra, OmegaConf, feature flags, 12-factor app  
`13` [Logging, Monitoring & Observability](https://karam-nus.github.io/software/13_logging_monitoring_and_observability) · structured logging, W&B, MLflow  
`14` [Error Handling & Debugging](https://karam-nus.github.io/software/14_error_handling_and_debugging) · pdb/ipdb, profiling, debugging distributed systems  
`15` [Code Review & Collaboration](https://karam-nus.github.io/software/15_code_review_and_collaboration) · PR best practices, trunk-based development, RFC process

**Systems & Performance**

`16` [Software Architecture](https://karam-nus.github.io/software/16_software_architecture) · monolith vs microservices, event-driven, ML pipeline architectures  
`17` [Performance & Profiling](https://karam-nus.github.io/software/17_performance_and_profiling) · cProfile, line_profiler, memory management, concurrency  
`18` [Security Best Practices](https://karam-nus.github.io/software/18_security_best_practices) · secrets management, OWASP basics, secure ML pipelines  
`19` [Data Engineering Basics](https://karam-nus.github.io/software/19_data_engineering_basics) · ETL/ELT, data validation, DVC, storage patterns  
`20` [ML System Design](https://karam-nus.github.io/software/20_ml_system_design) · model registry, feature stores, A/B testing, MLOps

**Appendices**

`A` [Package Management Deep Dive](https://karam-nus.github.io/software/appendix_a_package_management) · conda vs uv vs pip — complete workflows  
`B` [Unix & Shell Essentials](https://karam-nus.github.io/software/appendix_b_unix_and_shell) · shell scripting, SSH, tmux, cron, dotfiles  
`C` [VSCode Advanced Setup](https://karam-nus.github.io/software/appendix_c_vscode_setup) · extensions, debugging configs, remote dev, Copilot

</details>
