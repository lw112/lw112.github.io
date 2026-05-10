# lw112.github.io

Personal academic website for Laura Weihl, built with plain HTML and CSS - no frameworks, no build tools.

## Structure

```
lw112.github.io/
├── index.html          # About page (home)
├── publications.html
├── talks.html
├── posters.html
├── news.html
├── nav.html            # Shared navigation bar
├── sidebar.html        # Shared sidebar (photo, name, links)
├── style.css           # All styles
├── photo.jpg           # Profile photo
├── cv.pdf
└── img/
    ├── poster1.pdf
    └── poster1-thumb.jpg
```

## Editing content

- **Navigation links** — edit `nav.html`
- **Sidebar** (photo, name, affiliations, social links) — edit `sidebar.html`
- **About text** — edit `index.html`
- **Publications / Talks / Posters / News** — edit the respective HTML file

The index page automatically pulls the 4 most recent news items from `news.html`, so you only need to update news in one place.


## Local development

Because the nav and sidebar are loaded via `fetch()`, you need a local server to preview — just opening the HTML file directly won't work.

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Deployment

The site is hosted on GitHub Pages. Push to the `main` branch and changes go live at [lw112.github.io](https://lw112.github.io) within a minute or two.
