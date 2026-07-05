# k-npu-inference-recipes

Korean NPU and SoC inference recipe index for developers.

이 저장소는 FuriosaAI, Rebellions/RBLN, DEEPX 등 국산 NPU 생태계에서 공개된 추론 예제, OpenAI 호환 서버 튜토리얼, SDK 문서, Model Zoo, 모델 호환성 자료를 큐레이션한다.

## What This Repository Covers

- LLM 추론 서버
- OpenAI-compatible API 서버
- vLLM / Optimum / Runtime 기반 추론
- Embedding / Reranking / RAG 구성
- Vision / Object Detection / Segmentation
- Vision-Language / Multimodal inference
- Edge AI streaming inference

## Documents

| File | Purpose |
|---|---|
| [vendors.md](vendors.md) | 제조사별, 칩셋별, SDK별 추론 자료 색인 |
| [applications.md](applications.md) | 응용 분야별 추론 예제와 튜토리얼 색인 |

## Vendors

| Vendor | Chipset / Hardware | Main Stack | Main Recipes |
|---|---|---|---|
| FuriosaAI | RNGD | Furiosa-LLM, FXB, OpenAI-compatible server | LLM serving, embeddings, reranking, Qwen3-VL |
| Rebellions / RBLN | ATOM, ATOM+, ATOM-Max, RBLN-CA02/CA12/CA22/CA25 | RBLN SDK, Optimum RBLN, vLLM-RBLN | LLM, vLLM serving, HF model inference, vision, multimodal, diffusion |
| DEEPX | DX-M1 M.2, DXNN-compatible devices | DXNN SDK, DX-COM, DX-RT, DX-APP, DX-STREAM | Edge vision inference, detection, segmentation, pose, video analytics |

## Status Legend

| Status | Meaning |
|---|---|
| Official | Vendor documentation or vendor-owned repository |
| GitHub | Public source repository |
| Portal Required | Requires vendor portal, private package index, or hardware access |
| Needs Check | Public support is not clearly confirmed in official material |

## Inclusion Rules

- Include inference-only examples, tutorials, SDK guides, API server guides, and model zoo references.
- Exclude training-only, marketing-only, news-only, and unverifiable community claims.
- Mark hardware/account/private package requirements clearly.
- Mark unconfirmed model support as `Needs Check`.

## Suggested Repository Layout

```text
k-npu-inference-recipes/
  README.md
  vendors.md
  applications.md
  recipes/
    llm-chat/
    embeddings/
    reranking/
    vision/
    vision-language/
    streaming/
```

## Recipe Entry Template

```md
### Vendor / Model / Feature

| Field | Value |
|---|---|
| Vendor |  |
| Chipset |  |
| SDK / Runtime |  |
| Model |  |
| Task |  |
| Tutorial |  |
| Source Code |  |
| Status | Official / GitHub / Portal Required / Needs Check |
| Notes |  |
```

