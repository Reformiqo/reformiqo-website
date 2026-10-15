# reformiqo-website

Static landing page for **reformiqo.com**, deployed on CapRover (Hetzner `46.224.126.57`).

## What's here
- `index.html` — the landing page (served at `/`)
- `media/` — posters + testimonial videos (referenced with relative `media/...` paths)
- `captain-definition` — builds an `nginx:alpine` image that serves this folder

## How deploys work
This repo is connected to the CapRover app that serves `reformiqo.com`.
**Pushing to the `main` branch triggers an automatic rebuild + redeploy** via a CapRover webhook — no manual steps. Edit `index.html` or swap files in `media/`, commit, push, and the live site updates in ~1 minute.

## Edit locally
Just open `index.html` in a browser to preview. Keep media references relative (`media/<file>`).
