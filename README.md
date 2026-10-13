# site-preview

A single-page HTML template I use to mock up content sites quickly. Pure HTML, CSS and a tiny bit of vanilla JS — no build step, no framework, no dependencies. Open `index.html` in any browser and it works.

This folder is the version I have deployed on Cloudflare Pages. The twin copy in `AI项目1/site-preview/` is the local working version I iterate on before copying changes over.

## What's in it

```
site-preview/
├── index.html          # single-page site
├── assets/             # hero + gallery images
│   ├── hero.jpg
│   └── gallery-1.jpg … gallery-3.jpg
└── README.md
```

## How to use it

1. Keep `index.html` and the `assets/` folder together in the same directory.
2. Open `index.html` directly in a browser — double-click is fine.
3. Search for `示例文本` in `index.html` and replace each occurrence with your own copy.
4. To swap imagery, just overwrite the files in `assets/` with same-named replacements. The layout will stay intact.

## Deploying to Cloudflare Pages

There's no build step, so Cloudflare Pages can serve the folder as-is:

- Build command: *(leave empty)*
- Build output directory: `/`

Any commit to the connected branch is published automatically.

## Implementation notes

- The page is fully responsive and collapses to a single column below 960 px.
- The hamburger menu is a CSS overlay with a small JS toggle, no third-party code.
- All copy is hard-coded into `index.html` as placeholder text. If I needed real CMS-backed copy I'd reach for a static site generator, but for mockups this is faster than spinning one up.
