# HanziKey Website

Support and privacy pages for [HanziKey](https://apps.apple.com/), a
pop-up Mandarin dictionary for macOS.

## Pages

- **Landing** — `index.html` (plain HTML; uses `assets/css/style.css`).
- **Support** — `support.md` (rendered via `_layouts/default.html`).
- **Privacy** — `privacy.md` (rendered via `_layouts/default.html`).

All three share the same stylesheet and chrome.

## Structure

```
index.html             # landing page
support.md, privacy.md # markdown content pages
_layouts/default.html  # shared layout (header + footer + CSS link)
_config.yml            # Jekyll config; auto-injects layout: default
assets/css/style.css   # all site styles (tokens, components, content typography)
screenshots/           # icon.png + hover.png + others
CNAME                  # custom domain: www.hanzikey.com
```

## Deployment

Hosted on GitHub Pages. Pushes to `main` deploy automatically at
[www.hanzikey.com](https://www.hanzikey.com).

To preview locally:

```bash
bundle install --path vendor/bundle
bundle exec jekyll serve --livereload
```

Or for a fast preview of the landing only (skips Jekyll, markdown
pages won't render):

```bash
python3 -m http.server 4000
```
