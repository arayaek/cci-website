# Cosotic Chemicals Industries PLC — website

Static website (HTML, CSS and a little JavaScript) for the 200,000 t/yr chlor-alkali project in the Semera Industrial Zone, Afar, Ethiopia. Hosted with GitHub Pages from the `main` branch.

- `index.html` — the whole site
- `img/` — hero rendering and illustrative photos (Unsplash and Pexels licences)
- `video/` — six 7-second hero background clips (Pexels licence)
- `favicon.svg` — the logo mark

## Common edits (near the top of the script at the bottom of `index.html`)

| What | Where |
| --- | --- |
| Company name, used everywhere on the page | `var COMPANY = {...}` |
| Contact-form ID (FormSubmit; delivers to the advisor's inbox) | `var FORM_ID = '...'` |
| Project milestones and their status (`done`, `prog`, `next`, `plan`) | `var MILESTONES = [...]` |

## Contact form

The form sends messages through [FormSubmit](https://formsubmit.co) to the advisor's inbox using the `FORM_ID`. The **first** submission triggers an activation email from FormSubmit to that address. Click **Activate Form** in it once; after that, messages are delivered normally.

## Project vs. operating-company mode

The site presents the plant as a project under development. When the plant is operating, change `data-stage="project"` to `data-stage="operating"` (near the top of `<body>`). Project-only content (class `proj`) hides and company content (class `op`) shows.
