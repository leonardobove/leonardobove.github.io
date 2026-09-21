# leonardobove.github.io

[![deploy](https://github.com/leonardobove/leonardobove.github.io/actions/workflows/deploy.yml/badge.svg)](https://github.com/leonardobove/leonardobove.github.io/actions/workflows/deploy.yml)

Personal academic website for Leonardo Bove — Quantum Engineer at SQMS, Fermilab, and incoming Ph.D. student in Computer Science at Northwestern University.

Live at: <https://leonardobove.github.io>

Built with [Jekyll](https://jekyllrb.com/) using the [al-folio](https://github.com/alshedivat/al-folio) theme.

## Local development

```bash
bundle install
bundle exec jekyll serve
```

The site is then available at `http://localhost:4000`.

## Structure

- `_pages/about.md` — homepage / bio
- `_data/cv.yml` — CV content, rendered at `/cv/`
- `_news/` — short announcements shown on the homepage and `/news/`
- `_posts/` — blog posts, shown at `/blog/`
- `_projects/` — project pages, shown at `/projects/`

## Deployment

Pushing to `main` triggers [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml), which builds the site with Jekyll and publishes the result to the `gh-pages` branch via [`JamesIves/github-pages-deploy-action`](https://github.com/JamesIves/github-pages-deploy-action). GitHub Pages must be configured (Settings → Pages) to serve from the `gh-pages` branch.
