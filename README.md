# Caustic Chemical Industries PLC — concept website

Static concept site for internal review by the owners. Capacities, dates, certifications, locations and contacts are placeholders.

- `index.html` — the whole site (HTML, CSS and JS in one file)
- `img/` — hero rendering plus Unsplash stock photos (Unsplash License), to be replaced with real plant photos

Hosted with GitHub Pages from the `main` branch. Search-engine indexing is discouraged via `noindex` and `robots.txt`.

## Project vs. operating-company mode

The site currently presents the plant as **a project under development**. When the plant is operating, open `index.html`, find `data-stage="project"` (near the top of `<body>`) and change it to `data-stage="operating"`. Project-only content (class `proj`, e.g. the Project status section) hides and company content (class `op`) shows.

Project milestones are a list named `MILESTONES` near the top of the script at the bottom of `index.html`; set each one's status to `done`, `prog`, `next` or `plan`.
