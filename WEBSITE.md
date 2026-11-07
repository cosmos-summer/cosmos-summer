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

The workflow in `.github/workflows/deploy-pages.yml` deploys the repository on
every push to `main`.

1. Open the repository settings on GitHub.
2. Select **Pages**.
3. Set **Source** to **GitHub Actions**.

You can also run the deployment manually from the repository's **Actions** tab.
