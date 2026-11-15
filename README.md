# Vibewire Lab website

Static landing page for Vibewire Lab that links to the GitHub repositories of the Tale family apps:

- Talewell: https://github.com/Thunder21907/Talewell
- Talekin: https://github.com/Thunder21907/Talekin
- Talefire: https://github.com/Thunder21907/Talefire

There's no build step. It's plain HTML and CSS, plus the app icons in `assets/` (copied from `../Branding`).

## Preview locally

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

## Publish on GitHub Pages

1. Create a public repository, for example `Thunder21907/vibewirelab`, and push this folder's contents to its `main` branch.
   (If you name the repo `Thunder21907.github.io`, the site is served at `https://thunder21907.github.io/` instead of under `/vibewirelab/`.)
2. On GitHub, go to **Settings > Pages**, and under **Build and deployment** choose **Deploy from a branch**, `main`, `/ (root)`.
3. The site goes live at `https://thunder21907.github.io/vibewirelab/` after a minute or two.

All paths are relative, so the page works both at a domain root and under a sub-path. To use your own domain, add it in **Settings > Pages > Custom domain** (GitHub creates a `CNAME` file for you).

The `.nojekyll` file tells GitHub Pages to serve the files as they are, without running Jekyll.
