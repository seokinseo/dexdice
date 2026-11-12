# DexDICE project page draft

This folder is a self-contained, buildless project page for the NeurIPS 2026 camera-ready paper. It includes one selected trial per method from the physical mobile-robot evaluation, plus an exported manuscript PDF and two figures from the paper. The page is written in English for the research audience.

## Preview locally

From the repository root:

```sh
python3 -m http.server 8000 --directory site
```

Open `http://localhost:8000/`. The videos work without a build step.

## Publish to GitHub Pages

Published at https://seokinseo.github.io/dexdice-site/ from the `seokinseo/dexdice-site` repository (GitHub Pages, `main` branch, root).

For a standalone `<username>.github.io` repository, copy the contents of this folder into that repository's root, then enable Pages from the default branch. For an existing repository that keeps this `site/` folder, use a GitHub Actions Pages workflow that uploads `./site` as the artifact. GitHub Pages' branch-based source setting only accepts the repository root or `/docs`.

The page uses relative paths, so it works at either a user-site root or a project-site subpath. The Code links point to https://github.com/tzs930/dexdice.

## Assets and updates

- Paper links point to the arXiv PDF (https://arxiv.org/pdf/2611.09433). `assets/dexdice-neurips-2026.pdf` is no longer referenced by the page.
- `assets/images/method-overview.png`, `robot-arena.jpg`, and `controlled-*.png`: figures exported from the manuscript. The controlled-experiment plots open at full size when selected.
- `assets/videos/*.mp4`: compressed, representative clips from the five method folders under `mobile_video`; the page labels them as selected trials. The quantitative results summarize all ten trials per method.
- `assets/images/poster-*.png`: still frames for those clips.

The raw videos remain outside this folder. The five compressed clips are about 32 MB in total.
