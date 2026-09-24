# Digital Magnet Media — Exact Jekyll Source

This project is generated directly from the production HTML used by the live Digital Magnet Media preview. It preserves the four pages, visual layouts, original image assets, typography, clapboard and curtain entrance, animations, forms, navigation, shared company wordmark, and shared footer.

## Run locally

1. Install Ruby 3.1 or newer.
2. Run `bundle install`.
3. Run `bundle exec jekyll serve`.
4. Open `http://localhost:4000/`.

## Important files

- `index.html` — exact Home page source
- `about.html` — exact About page source
- `services.html` — exact Services & Works page source
- `contact.html` — exact Contact page source
- `_includes/footer.html` — the shared footer used by all pages
- `assets/css/site.scss` — shared footer styling in SCSS
- `static-original/` — untouched production HTML snapshots for direct comparison

Page-specific styling and JavaScript remain inline because that is how the production preview is implemented. The only extraction is the identical shared footer, moved into a Jekyll include and SCSS entry point.


## Image hosting

Recovered artwork is bundled in `assets/images/` and referenced with Jekyll’s `relative_url` filter so it works under the configured GitHub Pages base URL. Keep these files with the deployment. Some original Google `/aida/` URLs return HTTP 403; the remaining remote references require the original image files or replacement artwork. `static-original/` retains the original snapshots.
