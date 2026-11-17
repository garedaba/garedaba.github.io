# garedaba.github.io

Website source for [garedaba.github.io](https://garedaba.github.io/). 
| Page | URL | Code |
|---|---|---|
| Projects (landing) | `/` | – |
| μBrain atlas | `/micro-brain/` | [garedaba/micro-brain](https://github.com/garedaba/micro-brain) |
| About μBrain | `/micro-brain/about` | – |
| Cortical expansion | `/micro-brain/cortical_expansion/` | [garedaba/micro-brain](https://github.com/garedaba/micro-brain) |
| Prenatal network hubs | `/micro-brain/prenatal_hubs/` | [garedaba/prenatal-hubs](https://github.com/garedaba/prenatal-hubs) |
| Prenatal thalamus | `/micro-brain/prenatal_thalamus/` | [garedaba/prenatal-thalamus](https://github.com/garedaba/prenatal-thalamus) |

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
