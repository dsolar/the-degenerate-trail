# The Degenerate Trail

An Oregon Trail-inspired browser game about getting Nick home through Montreal nightlife.

## Play

The current hosted version is available at:

https://the-degenerate-trail.davidbsolar.chatgpt.site

## Run locally

The game is a static site with no build step. Serve the `dist` directory with any local web server:

```bash
python3 -m http.server 8000 --directory dist
```

Then open `http://localhost:8000`.

## Add it to WordPress

Upload the contents of `dist` to a directory on the WordPress server, or embed the hosted version in a Custom HTML block:

```html
<iframe
  src="https://the-degenerate-trail.davidbsolar.chatgpt.site"
  title="The Degenerate Trail"
  style="display:block;width:100%;height:850px;border:0"
  allow="fullscreen">
</iframe>
```

The hosted Site must be publicly accessible for an iframe on a public WordPress page.

## Project structure

- `dist/index.html`: page markup
- `dist/style.css`: layout and presentation
- `dist/game.js`: game state, movement, consequences, and endings
- `dist/encounters.js`: dialogue encounters and Nick-isms
- `dist/assets/nick-sprite.png`: character artwork

