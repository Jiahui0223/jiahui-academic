# jiahui-academic

Source for my academic site at **[academic.jiahui9923.com](https://academic.jiahui9923.com)**.

Research Assistant in the [Computer Vision Lab](https://www.cs.virginia.edu/) at the University of Virginia, working with Prof. Zezhou Cheng on 3D scene understanding, multi-frame perception, and transformer-based spatial reasoning.

## Stack

- [Jekyll](https://jekyllrb.com/) (Ruby static site generator)
- [al-folio](https://github.com/alshedivat/al-folio) academic theme (MIT licensed)
- Hosted on GitHub Pages, built via GitHub Actions on every push to `main`
- DNS: subdomain CNAME pointing at `jiahui0223.github.io`

## Local development

```bash
# Requires Docker Desktop
docker compose up
# Site at http://localhost:8080
```

Edits to most files hot-reload. Changes to `_config.yml` need a restart:

```bash
docker compose restart
```

## Where things live

| Path | What |
|---|---|
| `_pages/about.md` | Home page (bio, profile) |
| `_pages/projects.md` | Projects index |
| `_pages/publications.md` | Publications (driven by `_bibliography/papers.bib`) |
| `_pages/cv.md` | CV page (embeds `assets/pdf/Jiahui_Resume_*.pdf`) |
| `_projects/*.md` | One file per project card |
| `_news/*.md` | Recent updates shown on the home page |
| `_data/socials.yml` | Social profile usernames / links |
| `assets/css/main.scss` | Local style overrides (theme color, typography, custom components) |
| `_includes/`, `_layouts/` | Local overrides of upstream al-folio templates |
| `assets/img/` | Profile photo, project images, favicon |
| `.github/workflows/deploy.yml` | CI: build with Jekyll, publish to `gh-pages` |
| `CNAME` | Pins GitHub Pages to `academic.jiahui9923.com` |

## License

Site code is MIT (inherited from al-folio — see `LICENSE`).
All written content, photos, and personal materials are © Jiahui Zhang.
