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
| CV | `_data/cv.yml`, PDF in `assets/pdf/` |
| Blog posts | `_posts/*.md` |
| Social links | `_data/socials.yml` |
| Site settings | `_config.yml` |

Deployed by `.github/workflows/deploy.yml`: pushes to `master` build the site and force-push `_site` to the `gh-pages` branch, which GitHub Pages serves.
