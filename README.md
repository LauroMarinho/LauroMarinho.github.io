# lauromarinho.github.io

Personal portfolio — iOS developer. One static page, no build step, no dependencies.

```
index.html          the whole page
styles.css          the whole design
assets/screens/     app screenshots (see the README in there)
```

## Running it locally

Open `index.html` in a browser. That's it.

## Adding a screenshot

Drop a PNG into `assets/screens/` using the filenames listed in
[`assets/screens/README.md`](assets/screens/README.md). The page shows the image
automatically and hides the dashed placeholder — no code change needed.

## Adding an App Store link

Each app card has a `.links` block. Add a link next to the existing ones:

```html
<a class="link solid" href="https://apps.apple.com/app/idXXXXXXXXX" target="_blank" rel="noopener">
  Download on the App Store
</a>
```

There is an `<!-- APPSTORE:ARTISTLAB -->` marker on the ArtistLab card for exactly this.

## Deploying

GitHub Pages, served from the `main` branch root. Every push to `main` republishes.
