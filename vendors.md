# Vendors

제조사별, 칩셋별, SDK별 국산 NPU 추론 자료 색인이다.

## 1. FuriosaAI

### Chipset

| Chipset | Notes |
|---|---|
| RNGD | Data-center AI accelerator for LLM and agentic AI inference |

### Core Stack

| Component | Purpose | Link | Status |
|---|---|---|---|
| Furiosa-LLM Quick Start | Install and run Furiosa-LLM | [Quick Start with Furiosa-LLM](https://developer.furiosa.ai/latest/en/get_started/furiosa_llm.html) | Official |
| OpenAI-Compatible Server | Serve one model with OpenAI-compatible APIs | [OpenAI-Compatible Server](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html) | Official |
| Supported Models | Supported architectures and validated models | [Supported Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/supported_models.html) | Official |
| FuriosaAI Hugging Face | Pre-compiled FXB model repositories | [furiosa-ai on Hugging Face](https://huggingface.co/furiosa-ai) | Official |
| Furiosa SDK Cookbook | SDK examples and recipes | [FuriosaAI SDK Cookbook](https://github.com/furiosa-ai/furiosa-sdk-cookbook) | GitHub |

### Inference Recipes

| Feature | Model / Family | Tutorial | Notes | Status |
|---|---|---|---|---|
| Text generation | EXAONE 4.0, K-EXAONE, GPT-OSS, Llama 3.1/3.3, Solar Open, Qwen2.5, Qwen3, Qwen3-MoE | [Supported Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/supported_models.html) | Architecture list and validated FXB links | Official |
| Chat Completions API | Chat-template-compatible text models | [OpenAI-Compatible Server](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html) | `/v1/chat/completions` | Official |
| Completions API | Text generation models | [OpenAI-Compatible Server](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html) | `/v1/completions` | Official |
| Responses API | Chat-template-compatible models | [Responses API](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/responses-api.html) | OpenResponses-compatible API | Official |
| Embeddings | Qwen3-Embedding | [Supported Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/supported_models.html#pooling-models) | `/v1/embeddings` | Official |
| Reranking | Qwen3-Reranker | [OpenAI-Compatible Server](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html) | `/rerank`, `/v1/rerank`, `/v2/rerank` | Official |
| Similarity scoring | Qwen3-Reranker | [OpenAI-Compatible Server](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html) | `/score`, `/v1/score` | Official |
| Tool calling | EXAONE 4.0, Qwen3-compatible models | [Tool Calling Support](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html#tool-calling-support) | `--enable-auto-tool-choice` | Official |
| Reasoning parser | Qwen3, DeepSeek-style reasoning models | [Reasoning Support](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html#reasoning-support) | Reasoning content handling | Official |
| Vision-language | Qwen3-VL | [Vision-Language Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/vision-language.html) | OpenAI-compatible image + text chat | Official |
| Container serving | Furiosa-LLM server container | [Server Container](https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html#launching-the-openai-compatible-server-container) | Docker deployment | Official |
| Kubernetes serving | Furiosa-LLM on Kubernetes | [Kubernetes Deployment](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/k8s_deployment.html) | Cluster deployment | Official |

### Model Shortlist

| Task | Model / Family | Link | Status |
|---|---|---|---|
| Korean / enterprise LLM | EXAONE 4.0 | [Supported Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/supported_models.html) | Official |
| Korean sovereign AI scale model | K-EXAONE | [Supported Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/supported_models.html) | Official |
| Open-weight reasoning / MoE | GPT-OSS | [Supported Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/supported_models.html) | Official |
| General chat | Llama 3.1 / 3.3 | [Supported Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/supported_models.html) | Official |
| Korean / global LLM | Solar Open | [Supported Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/supported_models.html) | Official |
| Reasoning / coding / chat | Qwen3 | [Qwen3 dense guide](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/models/qwen3.html) | Official |
| MoE LLM | Qwen3-MoE | [Qwen3-MoE guide](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/models/qwen3-moe.html) | Official |
| Embedding | Qwen3-Embedding | [Supported Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/supported_models.html) | Official |
| Reranking | Qwen3-Reranker | [Supported Models](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/supported_models.html) | Official |
| Vision-language | Qwen3-VL | [Qwen3-VL guide](https://developer.furiosa.ai/v2026.3.0/en/furiosa_llm/models/qwen3-vl.html) | Official |

## 2. Rebellions / RBLN

### Chipsets

| Chipset / Product Line | Notes |
|---|---|
| ATOM / RBLN-CA02 | Single-NPU examples in earlier Optimum RBLN docs |
| ATOM+ / RBLN-CA12, RBLN-CA22 | Multi-NPU and RSD examples |
| ATOM-Max / RBLN-CA25 | Larger model and multi-NPU target in recent docs |

### Core Stack

| Component | Purpose | Link | Status |
|---|---|---|---|
| RBLN SDK Quick Start | Setup, compile, inference, serving | [RBLN Quick Start](https://docs.rbln.ai/latest/getting_started/quick_start.html) | Official / Portal Required |
| Optimum RBLN | Hugging Face transformers and diffusers bridge | [Optimum RBLN Overview](https://docs.rbln.ai/latest/software/optimum/index.html) | Official / Portal Required |
| vLLM-RBLN | vLLM hardware plugin for RBLN NPU | [vLLM RBLN](https://docs.rbln.ai/latest/software/model_serving/vllm_support/index.html) | Official / Portal Required |
| OpenAI-compatible vLLM Server | Serve compiled RBLN model through vLLM API server | [OpenAI Compatible Server](https://docs.rbln.ai/latest/software/model_serving/vllm_support/tutorial/openai_api_server.html) | Official / Portal Required |
| RBLN Model Zoo | Public examples across HF, PyTorch, TensorFlow, C++, vLLM, serving | [RBLN Model Zoo](https://github.com/RBLN-SW/rbln-model-zoo) | GitHub |

### Inference Recipes

| Feature | Model / Family | Tutorial | Notes | Status |
|---|---|---|---|---|
| LLM text generation | Llama3, Qwen2.5, Qwen3, GPT-2, Gemma, OPT, Phi, T5, BART, EXAONE, Mi:dm, Mistral | [Optimum RBLN Overview](https://docs.rbln.ai/latest/software/optimum/index.html) | Compile and infer HF models | Official / Portal Required |
| vLLM serving | Llama3-8B, Llama3.1-8B, Qwen3-0.6B | [vLLM RBLN](https://docs.rbln.ai/latest/software/model_serving/vllm_support/index.html) | vLLM-RBLN path | Official / Portal Required |
| OpenAI-compatible API | Llama3-8B compiled with Optimum RBLN | [OpenAI Compatible Server](https://docs.rbln.ai/latest/software/model_serving/vllm_support/tutorial/openai_api_server.html) | `vllm serve ./compiled-model` | Official / Portal Required |
| Embedding / sentence similarity | Qwen3-Embedding, E5, LaBSE, KR-SBERT, BGE | [Optimum RBLN Overview](https://docs.rbln.ai/latest/software/optimum/index.html#transformers) | Retrieval and RAG embeddings | Official / Portal Required |
| Reranking | Qwen3-Reranker, BGE-Reranker | [Optimum RBLN Overview](https://docs.rbln.ai/latest/software/optimum/index.html#transformers) | Document reranking | Official / Portal Required |
| Vision classification | ResNet, ViT, DPT, Depth Anything V2 | [Optimum RBLN Overview](https://docs.rbln.ai/latest/software/optimum/index.html) | Vision inference APIs | Official / Portal Required |
| Object detection | YOLOv8 | [RBLN Profiler Example - YOLOv8](https://docs.rbln.ai/latest/software/profiler/examples/yolov8.html) | Profiling plus inference context | Official / Portal Required |
| Vision-language | Qwen2-VL, Qwen2.5-VL, Qwen3-VL, LLaVA, Idefics3, PaliGemma, Grounding DINO | [Optimum RBLN Overview](https://docs.rbln.ai/latest/software/optimum/index.html) | Image-text inference | Official / Portal Required |
| Qwen3-VL multimodal | Qwen3-VL-4B / 32B family | [Qwen3-VL API](https://docs.rbln.ai/latest/software/optimum/model_api/transformers/multimodal_model/qwen3_vl.html) | Image and video encoding | Official / Portal Required |
| Image generation | Stable Diffusion, SDXL, SD3, ControlNet, Cosmos, SVD, Kandinsky | [Optimum RBLN Diffusers](https://docs.rbln.ai/latest/software/optimum/index.html#diffusers) | Diffusers pipelines | Official / Portal Required |

### Model Zoo Shortcuts

| Category | Link | Status |
|---|---|---|
| Hugging Face examples | [rbln-model-zoo / huggingface](https://github.com/RBLN-SW/rbln-model-zoo/tree/main/huggingface) | GitHub |
| vLLM examples | [rbln-model-zoo / vllm](https://github.com/RBLN-SW/rbln-model-zoo/tree/main/vllm) | GitHub |
| Serving examples | [rbln-model-zoo / serving](https://github.com/RBLN-SW/rbln-model-zoo/tree/main/serving) | GitHub |
| PyTorch examples | [rbln-model-zoo / pytorch](https://github.com/RBLN-SW/rbln-model-zoo/tree/main/pytorch) | GitHub |
| TensorFlow examples | [rbln-model-zoo / tensorflow](https://github.com/RBLN-SW/rbln-model-zoo/tree/main/tensorflow) | GitHub |
| C++ examples | [rbln-model-zoo / cpp](https://github.com/RBLN-SW/rbln-model-zoo/tree/main/cpp) | GitHub |

## 3. DEEPX

### Chipsets

| Chipset / Module | Notes |
|---|---|
| DX-M1 M.2 | Public Model Zoo benchmark target in DEEPX developer page |
| DXNN-compatible devices | Target devices supported through DXNN SDK, DX-RT, DX-APP, and DX-STREAM |

### Core Stack

| Component | Purpose | Link | Status |
|---|---|---|---|
| DXNN SDK | Overall DEEPX SDK overview | [DXNN SDK](https://deepx.ai/products/dxnn-sdk/) | Official |
| DEEPX Developer Get Started | DXNN components and DX-Allsuite entry point | [Get Started](https://developer.deepx.ai/article/get-started/) | Official |
| DX-AllSuite | Version-aligned package for DXNN components | [dx-all-suite](https://github.com/DEEPX-AI/dx-all-suite) | GitHub |
| DX-Runtime | Runtime, driver, firmware, DX-APP, DX-STREAM | [dx-runtime](https://github.com/DEEPX-AI/dx-runtime) | GitHub |
| DX Model Zoo | Pre-compiled `.dxnn` model list and metrics | [DX Model Zoo](https://developer.deepx.ai/modelzoo/) | Official |

### Inference Recipes

| Feature | Model / Family | Tutorial | Notes | Status |
|---|---|---|---|---|
| ONNX to DXNN conversion | Custom ONNX models | [DEEPX Get Started](https://developer.deepx.ai/article/get-started/) | DX-COM compiles `.onnx` to `.dxnn` | Official |
| Runtime inference | `.dxnn` model files | [dx-runtime](https://github.com/DEEPX-AI/dx-runtime) | DX-RT with DX-APP examples | GitHub |
| Image classification | AlexNet, DenseNet, EfficientNet, MobileNet, RegNet | [DX Model Zoo](https://developer.deepx.ai/modelzoo/) | Precompiled model list and sample apps | Official |
| Object detection | YOLO-style and detection models in Model Zoo | [DX Model Zoo](https://developer.deepx.ai/modelzoo/) | Confirm exact model entries before pinning | Official |
| Segmentation | Segmentation models in Model Zoo | [DX Model Zoo](https://developer.deepx.ai/modelzoo/) | Edge vision inference | Official |
| Face / pose / tracking | Model Zoo and DX-APP demos | [DX Model Zoo](https://developer.deepx.ai/modelzoo/) | Camera analytics tutorials | Official |
| Video / streaming inference | GStreamer pipelines | [dx-runtime](https://github.com/DEEPX-AI/dx-runtime) | DX-STREAM integration | GitHub |
| LLM inference | Decoder LLMs | Not confirmed in official public DXNN material | Public docs are vision/ONNX/runtime centric | Needs Check |

### Notes

- Standard workflow: export model to ONNX, compile with DX-COM into `.dxnn`, run with DX-RT.
- Public DX Model Zoo is the safest starting point for reproducible vision inference.
- Add DEEPX LLM recipes only after a DEEPX-owned tutorial or repository confirms a runnable LLM inference flow.

