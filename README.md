# fermi-site

The fermi website: Jekyll 4, published to GitHub Pages by GitHub Actions.

## What writes what

- **fermi hub** writes `_data/releases.yml` and the cover images in `assets/releases/`, then commits
  and pushes them. Don't edit those by hand: the next publish from the hub replaces them. Their shape
  is described in `docs/releases.schema.json` in the hub's repository; field names are the hub's.
- **Everything else** (layouts, pages, styles) is edited here by hand.

## Run it locally

Needs Ruby 3.3 with DevKit (`C:\Ruby33-x64`) and Bundler.

```
bundle install
bundle exec jekyll serve
```

Then open http://127.0.0.1:4000/.

## Publishing

Every push to `main` builds and deploys the site (`.github/workflows/pages.yml`). One-time setup on
GitHub: **Settings → Pages → Build and deployment → Source: GitHub Actions**.

`planning/` (the SOP and mockups) is gitignored: it stays on this computer and is never published.
