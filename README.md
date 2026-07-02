# Hackney Depot — website

A 3-page static website for [Hackney Depot](https://www.hackneydepot.com), 5 Sheep Lane, London E8 4QS.

- `index.html` — what Hackney Depot is
- `hire.html` — Main Hall (events, workshops, filming) and White Studio (photoshoots)
- `studios.html` — the tenants
- `css/style.css` — the one stylesheet
- `js/main.js` — mobile nav toggle only
- `images/` — optimised web images
- `image_selection/` — original source images (not referenced by the site)

No build step. Plain HTML/CSS/JS.

## Run locally

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000

## Deploy to Render

1. Push this folder to a GitHub repository.
2. On [render.com](https://render.com): **New → Static Site**, connect the repo.
3. Leave the build command empty, set the publish directory to `.` (the included `render.yaml` configures this automatically if you use "New → Blueprint").

## Editing

- Tenants: edit the `<ul class="tenants">` list in `studios.html`.
- Instagram grid: swap image files referenced in the `ig-grid` section of `index.html` (square-cropped by CSS, any aspect ratio works).
- Accent colour, spacing, type: CSS variables at the top of `css/style.css`.
