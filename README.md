# Vinayak's website

Website: https://vinayak42.github.io/

Repository: https://github.com/vinayak42/vinayak42.github.io

The current site uses plain HTML and CSS, with no build step or dependency installation.

## Edit locally

- `index.html`: biography, publications, teaching, and background.
- `style.css`: layout, colors, and typography.
- `portrait.png`: original portrait; the crop is controlled in CSS.
- `Vinayak-CV.pdf`: downloadable CV. This is a snapshot, not a live Overleaf connection.
- `fonts/ACaslonPro-Regular.otf`: the supplied font.

From this directory, run:

```sh
python3 -m http.server 8765 --bind 127.0.0.1
```

Open http://127.0.0.1:8765/ and refresh after editing. Press Ctrl-C in the terminal to stop the server. The Hindi font is loaded from Google Fonts; other site assets are stored in this repository.

## Publish updates

GitHub Pages should publish from `master` and `/ (root)` under **Settings → Pages → Deploy from a branch**. The `.nojekyll` file tells Pages to serve the static files directly.

Commit changes to `master` and push to `origin`. Check the Pages deployment under the repository's Actions tab, then visit the website.

Files from the earlier Academic Pages/Jekyll website remain in the repository for reference and to preserve existing downloadable assets. They are not needed to build the current homepage; do not run the old Ruby or npm build instructions for this site. The original export ZIP is kept locally and ignored by Git.
