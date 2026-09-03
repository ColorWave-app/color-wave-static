# color-wave-static

Minimal [Jekyll](https://jekyllrb.com/) static site with a single page: the
Privacy Policy for the **Color Wave** mobile app.

## Structure

- `PRIVACY_POLICY.md` — the only page, served as the site homepage (`/`).
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
