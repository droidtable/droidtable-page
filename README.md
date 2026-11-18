# droidtable-page

GitHub Pages site for [Droidtable](https://github.com/droidtable) — a touch-friendly
Android photo editor built on darktable's own processing engine.

Served at: **https://droidtable.github.io/droidtable-page/**

## Setup (one-time)

1. In this repository on GitHub: **Settings → Pages → Build and deployment → Source:
   "Deploy from a branch"**, branch `main`, folder `/ (root)` → Save.
2. Push `main` (see below). GitHub auto-deploys on every push; watch the **Actions**
   tab for the `pages-build-deployment` job.
3. Optional custom domain: add a `CNAME` file at the repo root with the domain,
   point DNS at GitHub Pages, then enable "Enforce HTTPS" in the Pages settings.

## Local workflow

The site is plain static HTML — no build step. Edit `index.html`, then:

```bash
git add -A
git commit -m "Update the page"
git push
```

## Content rules

This repository is public. Never commit private material from the app repository:
no test fixtures (RAW/XMP files), no `compatibility/local/` run artifacts, no local
paths or credentials. Link to the public fork `droidtable/darktable` for source and
engine packages instead of copying them here.
