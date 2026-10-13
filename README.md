# site-preview

A single-page HTML template (Chinese) intended as a quick preview/scaffold for a content site. Open `index.html` in any browser — no build step, no dependencies.

> The root `index.html` and `assets/` are the **deployed on Cloudflare Pages** version of this project. The twin copy under `AI项目1/site-preview/` is the local working copy.

## Layout

```
site-preview/
├── index.html          # Single-page site
├── assets/             # Hero + gallery images
│   ├── hero.jpg
│   └── gallery-1.jpg … gallery-3.jpg
└── README.md
```

## How to Use

1. Keep `index.html` and the `assets/` folder together in the same directory.
2. Open `index.html` directly in a browser (double-click works).
3. Replace any of the `示例文本` placeholders in `index.html` with your own copy.
4. Swap the images in `assets/` with same-named files to keep the layout intact.

## Notes

- Pure HTML + CSS + a tiny vanilla-JS overlay menu. No frameworks.
- Fully responsive: collapses to a single column below 960 px.
- `AI项目1/site-preview/` is a parallel copy used during local iteration; this folder is the one deployed to Cloudflare Pages.
