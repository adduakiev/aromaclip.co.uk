# AromaClip — website

Static website for **AromaClip**, a pocket nasal inhaler with natural BIO essential oils
(Rhinofilt GmbH, Berlin). Three blends: **Breathe**, **Focus**, **Sleep**.

## Pages

| File | Page |
|---|---|
| `index.html` | Home — collection, starter set, how to use, specifics |
| `breathe.html`, `focus.html`, `sleep.html` | Product pages |
| `story.html` | The AromaClip story and philosophy |
| `science.html` | The research behind AromaClip |
| `hotels.html` | Co-branded partnership for hotels |
| `cart.html`, `checkout.html`, `confirmation.html` | Bag, checkout (prototype, no payments processed) and order confirmation |

## How it works

- Plain HTML/CSS/JS — no build step, no dependencies. Every page is self-contained:
  images and videos are embedded, fonts load from Google Fonts.
- The bag is stored in the browser's `localStorage` (key `aromaclip_cart`).
- The "Watch how it works" video plays inline when the site is served over http(s);
  opened as a local file it opens the video on YouTube instead.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Publish with GitHub Pages

Repository → **Settings → Pages** → Source: *Deploy from a branch* → Branch: `main`, folder `/ (root)` → Save.
The site will be available at `https://<your-username>.github.io/<repository-name>/`.
