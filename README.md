# brainardphilemon.github.io

Source for <https://brainardphilemon.github.io>, built with [Jekyll](https://jekyllrb.com/)
and the [al-folio](https://github.com/alshedivat/al-folio) theme (v0.13-era layout).

## Where things live

| What | File |
|---|---|
| Home page bio | `_pages/about.md` |
| News | `_news/announcement_*.md` |
| Publications | `_bibliography/papers.bib` (`selected={true}` shows a paper on the home page) |
| Experience, projects, writings | `_pages/misc.md` |
| Blog posts | `_posts/` |
| CV PDF | `assets/pdf/cv.pdf` |
| Social links | `_data/socials.yml` |
| Site settings | `_config.yml` |

## Preview locally

Requires Docker and make:

```bash
make serve   # http://localhost:4000
```

## Publishing

Push to `main`. GitHub Actions builds the site and publishes it to the `gh-pages`
branch, which GitHub Pages serves.
