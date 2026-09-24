# color-wave-static

Minimal [Jekyll](https://jekyllrb.com/) static site for the **Color Wave**
mobile app: a home page and its Privacy Policy.

## Structure

- `index.md` — the home page, served at `/`.
- `privacy.md` — the Privacy Policy page.
- `_layouts/default.html` — minimal layout (centered container, no nav/footer).
- `assets/css/style.css` — minimal styling (bold titles, plain body text).
- `_config.yml`, `Gemfile` — Jekyll configuration, built with the
  `github-pages` gem.

## Local development

```bash
bundle install
bundle exec jekyll serve
```

Then open [http://localhost:4000](http://localhost:4000).

## Deployment

The site is hosted on **GitHub Pages**, built directly from this repository
(Settings → Pages → Deploy from branch).
