# agilityqa-com

Personal resume and consulting site for Christopher Lee, served at https://agilityqa.com/.

A static site with no build step:

- `index.html` holds all content (hero, audit matrix, engagements, experience, projects, credentials, contact)
- `assets/styles.css` holds all styling; colors and type sizes are CSS variables at the top
- `favicon.svg`

## Preview locally

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Content sources

Experience, credentials and the about copy come from LinkedIn (linkedin.com/in/christopher-mark-lee).
Projects come from github.com/christophermarklee and github.com/ergoshear.

## Deploy

`.github/workflows/pages.yml` publishes the site to GitHub Pages on every push to `main` (or manually from the Actions tab). Only `index.html`, `favicon.svg` and `assets/` are published; add new top-level files to the "Assemble site" step.

One-time setup in the repository settings, under Pages:

1. Set Source to "GitHub Actions".
2. Set the custom domain to `agilityqa.com` and point DNS at GitHub Pages.
