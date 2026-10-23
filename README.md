# Walk me home

Harsh Nagrani's interactive portfolio. A student walks home from school after the 4:00 PM bell, and scrolling moves him along the road as the afternoon turns to dusk.

- **Five checkpoints:** About (notice board), Work (office block), Projects (workshop), Skills (library) and Contact (home). Click a marker to open each one.
- **Arcade Lane:** a detour between the workshop and the library with three playable games. They are Tennis vs Harsh, Gully cricket and a Uttarayan kite fight.
- **Extras:** green commits to collect along the way, honking autos, a chai stall, and a text-only view for quick reading.

## Stack

It is a single static `index.html` with no build step. The 3D scene uses [three.js](https://threejs.org) (r160, loaded from jsDelivr), and the games are plain Canvas 2D with Web Audio for sound.

## Run locally

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy

Import the repo into Vercel as a static site, with Framework Preset "Other" and no build command. Netlify and GitHub Pages also work as is.

## Deep links

Add one of these to the URL to open a stop directly: `#about`, `#work`, `#projects`, `#skills`, `#contact`, `#arcade`, `#tennis`, `#cricket` or `#kites`.
