# HUPcycle — Interactive Prototype

Finland's first national hub for textile upcycling. An interactive investor/partner prototype built as a single-file HTML site with no external dependencies.

**Live demo:** `https://<your-username>.github.io/hupcycle`

---

## File structure

```
hupcycle/
├── index.html              # Main prototype (entry point)
├── hupcycle-prototype.html # Working copy
├── .nojekyll               # Disables Jekyll — required for GitHub Pages
├── README.md
└── img/                    # Extracted photos from LSJH tExtended webinar
    ├── denim-bales.jpeg
    ├── lace-seconds.jpeg
    ├── rolf-runway-grid.jpeg
    ├── ervin-portrait.jpeg
    ├── ervin-garment.jpeg
    ├── ervin-bedding.jpeg
    ├── ervin-model.jpeg
    ├── fashion-1.jpeg … fashion-4.jpeg
    ├── workshop.jpeg
    ├── warehouse-1.jpeg
    ├── warehouse-2.jpeg
    ├── clothes-rack.jpeg
    ├── clothes-rack-color.jpeg
    ├── reuse-dress.jpeg
    └── … (additional extracted images)
```

---

## Deploy to GitHub Pages

### First time

1. Create a new repository on GitHub (e.g. `hupcycle`)
2. In your terminal, navigate to this folder and run:

```bash
git init
git add .
git commit -m "Initial HUPcycle prototype"
git branch -M main
git remote add origin https://github.com/<your-username>/hupcycle.git
git push -u origin main
```

3. Go to your repository on GitHub → **Settings** → **Pages**
4. Under *Source*, select **Deploy from a branch**
5. Choose **main** branch, **/ (root)** folder → click **Save**
6. Your site will be live at `https://<your-username>.github.io/hupcycle` within a minute or two

### Subsequent updates

```bash
git add .
git commit -m "Update prototype"
git push
```

GitHub Pages will automatically re-deploy on every push to `main`.

---

## Notes

- The prototype is fully self-contained — no npm, no build step, no external CDN dependencies
- All images are in `img/` and referenced with relative paths, so they work both locally and when hosted
- Arrow keys navigate between sections (presentation mode)
- The `.nojekyll` file is required — without it, GitHub Pages runs Jekyll and may fail on files with underscores or special characters in `img/`

---

*Photos sourced from the LSJH tExtended webinar, 1 April 2026. Contact: Miira Ojanen, LSJH / HUPcycle.*
