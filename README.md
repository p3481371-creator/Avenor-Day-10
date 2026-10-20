# AVENOR

Luxury perfume website: a scroll-driven film hero, a gold loading ritual, a scent finder and an optional ambient soundtrack.

## Pages

| Page | File |
| --- | --- |
| Home | `index.html` |
| Shop | `shop.html` |
| Our Story | `story.html` |
| Ingredients | `ingredients.html` |
| Journal | `journal.html` |
| Contact | `contact.html` |

## Assets

- `img/` holds the photography (WebP, full resolution).
- `film/` holds the 768 frames of the home film at 1280×720, two frames per file.

## Run locally

It is a static site with no build step. Serve the folder with any static server, for example:

```
python3 -m http.server 8000
```

Then open http://localhost:8000. Opening `index.html` straight from disk will not load the film frames, because browsers block those requests on `file://`.

## Deploy

Works as-is on Vercel, Netlify or GitHub Pages: point the host at the repository root, with no build command.

## External libraries

Lenis 1.1.13 (smooth scrolling) loads from jsDelivr at a pinned version. Fonts come from Google Fonts (Cormorant Garamond, Jost).
