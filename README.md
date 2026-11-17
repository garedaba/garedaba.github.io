# garedaba.github.io

Website source for the [μBrain](https://garedaba.github.io/micro-brain/) atlas and the studies built on it. Code for each study lives in its own repository; this repo only holds the website.

| Page | URL | Code |
|---|---|---|
| Redirect to μBrain | `/` | – |
| μBrain atlas | `/micro-brain/` | [garedaba/micro-brain](https://github.com/garedaba/micro-brain) |
| About μBrain | `/micro-brain/about` | – |
| Cortical expansion | `/micro-brain/cortical_expansion/` | [garedaba/micro-brain](https://github.com/garedaba/micro-brain) (`ANALYSIS/`) |
| Prenatal network hubs | `/micro-brain/prenatal_hubs/` | [garedaba/prenatal-hubs](https://github.com/garedaba/prenatal-hubs) |
| Prenatal thalamus | `/micro-brain/prenatal_thalamus/` | [garedaba/prenatal-thalamus](https://github.com/garedaba/prenatal-thalamus) |

## Going live (one-off)

1. Create a **public** repository named exactly `garedaba.github.io` and push this folder to its `main` branch.
2. In that repo: **Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)`**.
3. In **garedaba/micro-brain**: **Settings → Pages → Unpublish site** (or set the source to *None*).
   Until you do this, the old project site keeps serving `/micro-brain/` and takes priority over the new pages.
4. Leave `docs/` in `micro-brain` alone: its README embeds images from `docs/assets/images/`.
5. Optional: set the **Website** field in each code repo's *About* box to its page above (a settings change, no commit).

## Adding a new μBrain study

1. Copy `micro-brain/prenatal_hubs/` to `micro-brain/<new_study>/` and edit `index.md` (front matter `links:` drive the sidebar buttons).
2. Add an entry to `_data/microbrain_studies.yml`; it then appears in the sidebar of every μBrain page and on both landing pages.

## Preview locally

```
bundle install
bundle exec jekyll serve
```

## Structure

```
_config.yml                    site settings, Minimal theme (pages-themes/minimal@v0.2.0)
_layouts/default.html          Minimal layout with per-page sidebar links + studies list
_data/microbrain_studies.yml   list of studies built on μBrain
index.md                       landing page
micro-brain/                   μBrain pages and images (same URLs as the old site)
  cortical_expansion/
  prenatal_hubs/
  prenatal_thalamus/
```
