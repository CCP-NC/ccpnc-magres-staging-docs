# Magres Database Documentation

Source for the user documentation site, built with [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) and deployed to GitHub Pages via Actions on push to `main`.

## Layout

- `docs/` — the documentation content (Markdown), organized to match the site's user flow: getting started → search → results → datasets → upload → metadata update → reference/FAQ.
- `docs/assets/screenshots/` — cropped/annotated screenshots actually used in the published docs.
- `raw-materials/` — screenshots and the legacy FAQ page as provided for reference; not published, not linked from `mkdocs.yml`.
- `mkdocs.yml` — site config, theme, and navigation.
- `.github/workflows/deploy-docs.yml` — builds and deploys the site on every push to `main`.

## Local preview

```bash
pip install -r requirements.txt
mkdocs serve
```

Then open http://127.0.0.1:8000.

## Before first deploy

- Replace `REPLACE_ORG` / `REPLACE_REPO` in `mkdocs.yml` with the actual GitHub org and repo name.
- In the repo's Settings → Pages, set the source to the `gh-pages` branch (created automatically by the workflow after its first run).
