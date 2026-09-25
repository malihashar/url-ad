# url-ad

Paste a product URL → nine static ads with **Krea 2 Identity Edit** via the same `headswap_V2` Drive setup as face-swap (no HF token cell).

## Colab (general pipeline)

[Open in Google Colab](https://colab.research.google.com/github/malihashar/url-ad/blob/main/colab/url_to_ads_any.ipynb)

1. Runtime → **GPU**
2. Run cell **1** (mounts Drive; **skips re-download** if models already on Drive)
3. Cells **2–5** = one URL · cell **6** = batch three product types (denim / shorts / bag)
4. Krea = visuals only · Montserrat overlay mid-frame · hard **one person / product-only** rules

Notebook: [`colab/url_to_ads_any.ipynb`](colab/url_to_ads_any.ipynb)

Older prototype: [`colab/url_to_ads_krea2.ipynb`](colab/url_to_ads_krea2.ipynb)

## Docs

- [`research/ROADBLOCKS.md`](research/ROADBLOCKS.md)
- [`research/DEMO_URLS.md`](research/DEMO_URLS.md)
