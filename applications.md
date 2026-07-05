# Applications

응용 분야별 국산 NPU 추론 예제와 튜토리얼 색인이다.

## 1. LLM Chat / Text Generation

| Vendor | Chipset | Stack | Model / Family | Tutorial | Status |
|---|---|---|---|---|---|
| FuriosaAI | RNGD | Furiosa-LLM | EXAONE 4.0, K-EXAONE, GPT-OSS, Llama, Solar, Qwen | [Supported Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/supported_models.html) | Official |
| FuriosaAI | RNGD | Furiosa-LLM server | OpenAI-compatible chat models | [OpenAI-Compatible Server](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html) | Official |
| Rebellions / RBLN | ATOM / ATOM+ / ATOM-Max | Optimum RBLN | Llama3, Qwen, Gemma, OPT, Phi, T5, BART, EXAONE, Mi:dm, Mistral | [Optimum RBLN Overview](https://docs.rbln.ai/latest/software/optimum/index.html) | Official / Portal Required |
| Rebellions / RBLN | RBLN NPU | vLLM-RBLN | Llama3-8B, Llama3.1-8B, Qwen3-0.6B | [vLLM RBLN](https://docs.rbln.ai/latest/software/model_serving/vllm_support/index.html) | Official / Portal Required |
| DEEPX | DXNN-compatible devices | DXNN | Decoder LLMs | Not confirmed in official public DXNN material | Needs Check |

## 2. OpenAI-Compatible API Server

| Vendor | Runtime | API / Feature | Tutorial | Status |
|---|---|---|---|---|
| FuriosaAI | Furiosa-LLM | `/v1/chat/completions`, `/v1/completions`, `/v1/responses`, `/v1/embeddings` | [OpenAI-Compatible Server](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html) | Official |
| FuriosaAI | Furiosa-LLM | `/score`, `/rerank`, `/v1/rerank`, `/v2/rerank` | [OpenAI-Compatible Server](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html) | Official |
| Rebellions / RBLN | vLLM-RBLN | OpenAI-compatible HTTP server | [OpenAI Compatible Server](https://docs.rbln.ai/latest/software/model_serving/vllm_support/tutorial/openai_api_server.html) | Official / Portal Required |
| DEEPX | DX-RT / DX-STREAM | OpenAI-compatible LLM server | Not confirmed in official public material | Needs Check |

## 3. Embedding / Reranking / RAG

| Vendor | Stack | Model / Family | Task | Tutorial | Status |
|---|---|---|---|---|---|
| FuriosaAI | Furiosa-LLM | Qwen3-Embedding | Embedding | [Supported Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/supported_models.html#pooling-models) | Official |
| FuriosaAI | Furiosa-LLM | Qwen3-Reranker | Reranking, scoring | [OpenAI-Compatible Server](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html) | Official |
| Rebellions / RBLN | Optimum RBLN | Qwen3-Embedding, E5, LaBSE, KR-SBERT, BGE | Sentence similarity, retrieval | [Optimum RBLN Overview](https://docs.rbln.ai/latest/software/optimum/index.html#transformers) | Official / Portal Required |
| Rebellions / RBLN | Optimum RBLN | Qwen3-Reranker, BGE-Reranker | Document reranking | [Optimum RBLN Overview](https://docs.rbln.ai/latest/software/optimum/index.html#transformers) | Official / Portal Required |
| DEEPX | DXNN | Embedding / reranking models | RAG support | Not confirmed in official public material | Needs Check |

## 4. Tool Calling / Agentic AI

| Vendor | Stack | Model / Family | Tutorial | Status |
|---|---|---|---|---|
| FuriosaAI | Furiosa-LLM | EXAONE 4.0 and compatible tool-calling models | [Tool Calling Support](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html#tool-calling-support) | Official |
| FuriosaAI | Furiosa-LLM | Qwen3-MoE, Qwen3-Coder | [Qwen3-MoE guide](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/models/qwen3-moe.html) | Official |
| Rebellions / RBLN | Optimum RBLN / vLLM-RBLN | Qwen and Llama-family LLMs | [vLLM RBLN](https://docs.rbln.ai/latest/software/model_serving/vllm_support/index.html) | Official / Portal Required |
| DEEPX | DXNN | Agentic LLM | Not confirmed in official public material | Needs Check |

## 5. Vision-Language / Multimodal

| Vendor | Stack | Model / Family | Input / Output | Tutorial | Status |
|---|---|---|---|---|---|
| FuriosaAI | Furiosa-LLM | Qwen3-VL | Text + image to text | [Vision-Language Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/vision-language.html) | Official |
| Rebellions / RBLN | Optimum RBLN | Qwen2-VL, Qwen2.5-VL, Qwen3-VL, LLaVA, Idefics3, PaliGemma, Grounding DINO | Image-text inference | [Optimum RBLN Overview](https://docs.rbln.ai/latest/software/optimum/index.html) | Official / Portal Required |
| Rebellions / RBLN | Optimum RBLN | Qwen3-VL | Image / video encoding and conditional generation | [Qwen3-VL API](https://docs.rbln.ai/latest/software/optimum/model_api/transformers/multimodal_model/qwen3_vl.html) | Official / Portal Required |
| DEEPX | DXNN | Vision-language models | Needs Check | Not confirmed in official public material | Needs Check |

## 6. Vision Classification / Object Detection / Segmentation

| Vendor | Stack | Model / Family | Task | Tutorial | Status |
|---|---|---|---|---|---|
| Rebellions / RBLN | Optimum RBLN | ResNet, ViT, DPT, Depth Anything V2 | Classification, depth, vision inference | [Optimum RBLN Overview](https://docs.rbln.ai/latest/software/optimum/index.html) | Official / Portal Required |
| Rebellions / RBLN | RBLN Profiler / Model Zoo | YOLOv8 | Object detection | [YOLOv8 Profiler Example](https://docs.rbln.ai/latest/software/profiler/examples/yolov8.html) | Official / Portal Required |
| Rebellions / RBLN | RBLN Model Zoo | PyTorch, TensorFlow, C++, HF examples | Vision examples | [RBLN Model Zoo](https://github.com/RBLN-SW/rbln-model-zoo) | GitHub |
| DEEPX | DXNN / DX-RT | AlexNet, DenseNet, EfficientNet, MobileNet, RegNet | Image classification | [DX Model Zoo](https://developer.deepx.ai/modelzoo/) | Official |
| DEEPX | DXNN / DX-RT | YOLO-style, segmentation, pose, tracking models | Detection, segmentation, pose, video analytics | [DX Model Zoo](https://developer.deepx.ai/modelzoo/) | Official |
| FuriosaAI | Furiosa-LLM | Vision classification / detection | Needs Check | Not primary public focus in Furiosa-LLM docs | Needs Check |

## 7. Image Generation / Diffusion

| Vendor | Stack | Model / Family | Tutorial | Status |
|---|---|---|---|---|
| Rebellions / RBLN | Optimum RBLN Diffusers | Stable Diffusion, SDXL, SD3, ControlNet, Cosmos, SVD, Kandinsky | [Optimum RBLN Diffusers](https://docs.rbln.ai/latest/software/optimum/index.html#diffusers) | Official / Portal Required |
| FuriosaAI | Furiosa-LLM | Diffusion models | Not confirmed in current Furiosa-LLM public recipe set | Needs Check |
| DEEPX | DXNN | Diffusion models | Not confirmed in official public material | Needs Check |

## 8. Edge Video / Streaming

| Vendor | Stack | Use Case | Tutorial | Status |
|---|---|---|---|---|
| DEEPX | DX-STREAM / GStreamer | Video analytics, camera inference pipeline | [dx-runtime](https://github.com/DEEPX-AI/dx-runtime) | GitHub |
| DEEPX | DX-APP / DX-RT | Edge vision inference apps | [DX Model Zoo](https://developer.deepx.ai/modelzoo/) | Official |
| Rebellions / RBLN | Serving stack | Server-side model serving | [vLLM RBLN](https://docs.rbln.ai/latest/software/model_serving/vllm_support/index.html) | Official / Portal Required |
| FuriosaAI | Furiosa-LLM | LLM server deployment | [Furiosa-LLM OpenAI-Compatible Server](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html) | Official |

## 9. Deployment / Serving

| Vendor | Deployment Mode | Link | Status |
|---|---|---|---|
| FuriosaAI | Local OpenAI-compatible server | [OpenAI-Compatible Server](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html) | Official |
| FuriosaAI | Containerized server | [Server Container](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html#launching-the-openai-compatible-server-container) | Official |
| FuriosaAI | Kubernetes | [Kubernetes Deployment](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/k8s_deployment.html) | Official |
| Rebellions / RBLN | vLLM server | [vLLM RBLN](https://docs.rbln.ai/latest/software/model_serving/vllm_support/index.html) | Official / Portal Required |
| Rebellions / RBLN | OpenAI-compatible server | [OpenAI Compatible Server](https://docs.rbln.ai/latest/software/model_serving/vllm_support/tutorial/openai_api_server.html) | Official / Portal Required |
| Rebellions / RBLN | Triton / TorchServe / Ray Serve | [RBLN Model Serving](https://docs.rbln.ai/latest/software/model_serving/vllm_support/index.html) | Official / Portal Required |
| DEEPX | Local runtime | [dx-runtime](https://github.com/DEEPX-AI/dx-runtime) | GitHub |
| DEEPX | GStreamer streaming | [dx-runtime](https://github.com/DEEPX-AI/dx-runtime) | GitHub |
