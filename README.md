# junhyungahn.github.io

Personal academic website of Junhyung Ahn, built with [al-folio](https://github.com/alshedivat/al-folio) (Jekyll).

## Local development

```bash
bundle install
bundle exec jekyll serve   # http://localhost:4000
```

## Where content lives

| What | File |
| --- | --- |
| Bio, profile photo block | `_pages/about.md` |
| News items | `_news/*.md` |
| Publications | `_bibliography/papers.bib` (`selected={true}` puts a paper on the front page) |
| CV | `_data/cv.yml`, PDF in `assets/pdf/`, layout in `_includes/cv/render.liquid` (overrides the al_folio_cv gem template) |
| Social links | `_data/socials.yml` |
| Site settings | `_config.yml` |
| Local CSS overrides | `_sass/_local.scss` (loaded from the shadowed `assets/css/main.scss`) |

Deployed by `.github/workflows/deploy.yml`: pushes to `master` build the site and force-push `_site` to the `gh-pages` branch, which GitHub Pages serves.
