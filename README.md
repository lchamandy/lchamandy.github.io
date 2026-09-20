# Academic homepage (GitHub Pages)

Plain HTML and CSS with no build step. It uses Bootstrap 5, Font Awesome and the Poppins font, loaded from public CDNs, so the pages need an internet connection to look right.

| File | Purpose |
|---|---|
| `index.html` | Home: banner, section cards, opportunities, contact, footer |
| `research.html` | Overview cards, jump chips, and one section per research theme |
| `publications.html` | Publications grouped by year |
| `talks.html` | Talks grouped by year |
| `students.html` | Current and past students |
| `bio.html` | Short bio, positions, education |
| `assets/style.css` | All custom styling. Colours are variables at the top |
| `images/` | Your figures and photos. `placeholder.svg` is a stand-in |
| `cv/` | Put your CV here as `Curriculum_Vitae.pdf` |

## Updating an existing repo

Replace these files (upload with the same names and paths, then commit):
`index.html`, `research.html`, `publications.html`, `talks.html`, `students.html`, `bio.html`, `assets/style.css`, `images/placeholder.svg`.

## Fill in your details

Search all files for these and replace them:

- `Position title`
- `XX`, `XXXX`, `20XX` (counts, dates)
- The ADS, Google Scholar, ORCID and LinkedIn links (in `index.html` and the footers)
- All the placeholder text on each page

In `research.html`, copy a whole `<section class="research-theme">` block to add a theme, and add a matching chip in the `theme-nav` section.

## Photos (optional)

- **Banner portrait:** save a photo as `images/portrait.jpg`, then remove the comment markers around the `<img class="banner-portrait">` line in `index.html`.
- **Banner background:** save a wide image as `images/banner.jpg`, then in `assets/style.css` set `--banner-image: url("../images/banner.jpg");` and `--banner-overlay: 0.6;`.
- **Card backgrounds:** add `style="background-image: url(images/your-photo.jpg)"` to a card's `<a class="dls-card">` tag.
- **Research figures:** replace `images/placeholder.svg` in each `<img>` with your own file and update the `alt` text.

## Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.
