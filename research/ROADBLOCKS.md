# Roadblocks — URL → Nine Ads (Krea 2 Colab)

## Model / edit path
- **Identity Edit LoRA** (`conradlocke/krea2-identity-edit`) requires **ComfyUI-Krea2Edit** dual conditioning (VAE tokens + grounded Qwen3-VL). Stock `Krea2Pipeline` is **text-to-image only**.
- Colab mitigation: **Krea 2 Turbo T2I + optional product photo composite** so product identity stays recognizable without ComfyUI.
- **Ideogram 4** open weights: strong text, **no local product-edit API** — out of scope.

## Runtime
- HF **gated** download for `krea/Krea-2-Turbo` — must accept license + `HF_TOKEN`.
- VRAM: 12B DiT — prefer A100/L4; T4 uses `enable_model_cpu_offload()` (slower).
- Turbo settings: `steps=8`, `guidance_scale=0.0`.

## Extraction
- Brand PDPs (Allbirds, Amazon) often **block Colab/datacenter IPs**.
- Default demo URL (Shopify, JSON-LD friendly):  
  `https://satoshi-demo.myshopify.com/products/classic-straight-jeans`
- Notebook auto-falls back to that demo if the pasted URL fails.

## Quality
- Krea typography is weaker than GPT Image 2 / Ideogram — keep headlines short; QA reject illegible text.
- Composite improves product lock; layout/text still model-dependent.
