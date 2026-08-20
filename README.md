# personal-website

My personal website — plain HTML and CSS, no build step.

## Structure

```
index.html        # the page
css/styles.css    # all styles (design tokens at the top)
```

## Running it locally

Open `index.html` in a browser, or serve it so relative paths behave like they
will in production:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Editing

- Content lives in `index.html`. The placeholder copy in the hero, About,
  Projects, and Contact sections is meant to be replaced.
- Colors, spacing, and the max content width are CSS custom properties at the
  top of `css/styles.css`. Change them there rather than in individual rules.
- Dark mode follows the OS setting via `prefers-color-scheme` — update both
  token blocks when adding a new color.

## Deploying

Any static host works. For GitHub Pages: push to `main`, then in the repo's
**Settings → Pages**, set the source to the `main` branch, root directory.

## TODO

- [ ] Replace placeholder copy and links
- [ ] Add a favicon
- [ ] Add real project entries
