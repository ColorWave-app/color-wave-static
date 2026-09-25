# Copilot Instructions — color-wave-static

## What this project is

A minimal **Jekyll static site** for the "Color Wave" mobile app: a home page
and its Privacy Policy. The site has **exactly two pages**.

## Structure

- `index.md` — the home page (`permalink: /`). Presents Color Wave and links
  to the app store (currently a `#` placeholder).
- `privacy.md` — the Privacy Policy page. This
  file is the source of truth for the legal text and the page content.
- `_layouts/default.html` — the only layout. Wraps page content in a single
  centered `.container` div. Do not add nav bars, footers, or extra chrome.
- `assets/css/style.css` — minimal styling using CSS variables for the app's
  brand colors (pink/yellow/blue/maroon/teal), Plus Jakarta Sans headings, a
  `.hero` + `.store-buttons` layout, and a `.site-footer` style, ~700px
  max-width container. Keep it minimal; do not introduce a CSS framework or
  theme.
- `_config.yml` — Jekyll config (title, description, kramdown). No plugins
  beyond what `github-pages` gem provides.
- `Gemfile` — uses the `github-pages` gem so local builds match GitHub Pages'
  hosted build.

## Conventions / rules for changes

- **This site has two pages: `/` and `/privacy`.** Do not add new pages, blog
  posts, collections, or navigation unless explicitly asked.
- Keep the layout minimalist: no added visual complexity, animations, or
  third-party JS/CSS.
- Legal text in `policy.md` should only be edited when the user asks
  to change the policy content itself. Do not rephrase or restructure the
  policy without an explicit request.
- When editing `index.md` or `policy.md`, preserve the YAML front
  matter (`layout`, `title`, `permalink`) at the top of the file.

## Build & preview

```bash
bundle install
bundle exec jekyll serve
```

Site is served at `http://localhost:4000`.

## Deployment

Hosted via **Netlify**, built from the repo. Custom domain `color-wave.fr`
(purchased on Hostinger) is pointed at Netlify via DNS. No custom GitHub
Actions workflow is used unless the
user asks for one.
