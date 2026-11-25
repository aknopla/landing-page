# landing-page

The Aknopla landing page: static HTML, with no build step and no dependencies
to install.

| File | Page |
|---|---|
| `index.html` | Home |
| `technology.html` | Our technology |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

## Preview

```
python3 -m http.server 8000
```

Then open <http://localhost:8000/>.

## Publishing

GitHub Pages serves the root of `main` (Settings → Pages → Deploy from a
branch → `main`, `/ (root)`), so a push to `main` is a release. The address is
<https://aknopla.github.io/landing-page/>.

The site lives under `/landing-page/`, so links between pages and to assets
must be relative (`technology.html`, `logos/aws.svg`), never `/technology.html`.

## Placeholders

Search the HTML for `PLACEHOLDER` to find what is still to be replaced: the
logo, the hero video, the partner logos and the code-drawn visuals.
