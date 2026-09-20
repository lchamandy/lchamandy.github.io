# Academic homepage (GitHub Pages)

A plain HTML/CSS site with no build step. Pages:

| File | Purpose |
|---|---|
| `index.html` | Home: name, affiliation, profile links, CV button, section list, opportunities |
| `research.html` | Overview, jump links, and one section per research theme (text, key papers, figure) |
| `publications.html` | Publications grouped by year |
| `talks.html` | Talks grouped by year |
| `students.html` | Current and past students |
| `bio.html` | Short bio, positions, education |
| `assets/style.css` | All styling. Colours and fonts are variables at the top |
| `images/` | Your figures. `placeholder.svg` is a stand-in |
| `cv/` | Put your CV here as `Curriculum_Vitae.pdf` |

## 1. Fill in your details

Search all files for these strings and replace them:

- `Your Name`
- `your.email@niser.ac.in`
- `Position title`
- `XX` / `XXXX` / `20XX` (publication counts, dates)
- Profile links: ADS, Google Scholar, ORCID, LinkedIn and GitHub URLs (in `index.html` and the footers)

Then edit the text on each page. In `research.html`, copy a whole `<section class="theme">` block to add a theme, and add a matching link to the `chips` list at the top.

## 2. Publish on GitHub

1. Create a **public** repository named exactly `YOUR-GITHUB-USERNAME.github.io`.
2. Upload every file and folder from this directory to the repository root (including the hidden `.nojekyll` file).
3. In the repository, open **Settings > Pages**, set **Source** to "Deploy from a branch", choose branch `main` and folder `/ (root)`, and save.
4. After a minute or two the site is live at `https://YOUR-GITHUB-USERNAME.github.io`.

Command-line version:

```bash
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/YOUR-GITHUB-USERNAME/YOUR-GITHUB-USERNAME.github.io.git
git push -u origin main
```

## 3. Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Notes

- Fonts (Literata, Public Sans) load from Google Fonts, with system fallbacks if offline.
- The site follows the reader's light or dark setting automatically.
- The navigation and footer are repeated in each HTML file, so a change to the menu needs to be made in all six pages.
