# Website guide

This repository includes a lightweight personal placeholder built with plain
HTML and CSS. It deploys directly to GitHub Pages without a build step.

## Customize the site

Before publishing, edit `index.html` to replace `Your Name`, the introductory
copy, `hello@example.com`, and the placeholder GitHub link with your own details.
The colors and typography are defined near the top of `styles.css`.

## Preview locally

Run a static server from the repository root:

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Deploy to GitHub Pages

The site is intended to live at <https://cosmos-summer.github.io>. GitHub requires
a user site at that root URL to use a repository named `cosmos-summer.github.io`.

The profile introduction and website therefore need separate repositories:

| Repository | Purpose |
| --- | --- |
| `cosmos-summer/cosmos-summer` | GitHub profile `README.md` |
| `cosmos-summer/cosmos-summer.github.io` | Website source and Pages workflow |

Move `index.html`, `styles.css`, `.nojekyll`, and `.github/workflows/deploy-pages.yml`
into the `cosmos-summer.github.io` repository. The workflow deploys the root of
that repository on every push to `main`.

In the website repository, open **Settings → Pages** and set **Source** to
**GitHub Actions**.

You can also run the deployment manually from the repository's **Actions** tab.
