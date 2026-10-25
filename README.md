# Walk me home

Harsh Nagrani's interactive portfolio. Harsh logs off at the office and walks home, and scrolling moves him along the road. In light mode the evening turns to dusk, and in dark mode it's a moonlit walk after a late deploy.

- **Six checkpoints:** About (notice board), Work (office block), Projects (workshop), Skills (library), Blogs (bookstore) and Contact (home). However hard you scroll, Harsh stops at each one; open it, or scroll again to walk on.
- **Proofs & Pages:** at the Blogs checkpoint you step inside a 3D bookstore. Each article is a book on the featured shelf, and pulling one out shows what it covers with a link to read it.
- **Arcade Lane:** a detour between the workshop and the library with three playable games. They are Tennis vs Harsh, Gully cricket and a Uttarayan kite fight.
- **Light and dark:** the walk opens in light mode, and a Night toggle switches the sky, lights, games and bookstore. The choice is remembered on each device.
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

Add one of these to the URL to open a stop directly: `#about`, `#work`, `#projects`, `#skills`, `#blogs`, `#contact`, `#arcade`, `#tennis`, `#cricket` or `#kites`.
