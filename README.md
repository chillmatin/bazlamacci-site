# Cüneyt F. Bazlamaçcı — academic website

A modernised version of the homepage of Prof. Dr. Cüneyt F. Bazlamaçcı
(Computer Engineering Department, Izmir Institute of Technology), built with
[Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio) theme.

All content is migrated from the original page at
<https://web.iyte.edu.tr/~cuneytbazlamacci/>.

## Structure

| Page | Source |
| --- | --- |
| about (home) | `_pages/about.md` |
| research | `_pages/research.md` |
| publications | `_bibliography/papers.bib` |
| students | `_pages/students.md` |
| teaching | `_pages/teaching.md` |
| cv | `_data/cv.yml` + `_pages/cv.md` |

Site-wide settings (name, contact details, URL) live in `_config.yml`;
contact and CV links live in `_data/socials.yml`.

## Local development

```bash
bundle install
bundle exec jekyll serve
```

Or with Docker:

```bash
docker compose up
```

## Deployment

Pushing to `main` triggers `.github/workflows/deploy.yml`, which builds the site
and publishes it to the `gh-pages` branch via GitHub Pages.
