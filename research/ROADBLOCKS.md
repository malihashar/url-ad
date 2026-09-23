# Roadblocks — URL → Nine Ads (Krea 2 / headswap_V2)

## Stack
- Uses `malihashar/headswap_V2` branch `face-swap-no-mask` (same as face_swap_no_mask Colab).
- Models from Drive: `/content/drive/MyDrive/headswap_V2/models` via `setup_colab.sh --krea2`.
- Generation: `Krea2IdentityEditPipeline.edit_single_image` (single product photo + instruction).

## No HF token cell
- Notebook does not call `huggingface_hub.login`.
- First-time setup still downloads weights through headswap scripts (may use HF under the hood once into Drive).

## Runtime
- Prefer A100; T4 slower. Cold load + 9 edits is long on T4.
- Brand PDPs (Allbirds/Amazon) may block Colab IPs → demo Shopify URL fallback.

## Ideogram
- Out of scope (no local product-edit graph).
