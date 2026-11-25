# sayumimuthu.github.io

Personal academic website of **Sayumi Muthukumarana**, built with [al-folio](https://github.com/alshedivat/al-folio) (Jekyll) and hosted on GitHub Pages.

Live site: <https://sayumimuthu.github.io>

## First-time deployment

1. Create a **public** repository named exactly `sayumimuthu.github.io` on GitHub (leave it empty: no README, no license).
2. In the new repository, open **Settings → Actions → General → Workflow permissions**, choose **Read and write permissions**, and save.
3. In this folder, run:

   ```bash
   git init -b main
   git add .
   git commit -m "Initial website"
   git remote add origin https://github.com/sayumimuthu/sayumimuthu.github.io.git
   git push -u origin main
   ```

4. Open the **Actions** tab and wait for the "Deploy site" run to finish (about 3 to 5 minutes). If it did not start, click **Deploy site → Run workflow**.
5. A `gh-pages` branch now exists. Go to **Settings → Pages**, set **Source: Deploy from a branch**, **Branch: `gh-pages` / (root)**, and save. Do not edit the `gh-pages` branch by hand.
6. After a minute or two the site is live at <https://sayumimuthu.github.io>.

Every later push to `main` rebuilds and redeploys the site automatically.

## Where to edit things

| What                                   | File                                                                              |
| -------------------------------------- | --------------------------------------------------------------------------------- |
| Home page bio, subtitle, photo caption | `_pages/about.md`                                                                 |
| Profile photo                          | `assets/img/prof_pic.jpg` (portrait, about 4:5)                                   |
| Publications                           | `_bibliography/papers.bib` (BibTeX; `selected = {true}` shows it on the homepage) |
| Publication thumbnails                 | `assets/img/publication_preview/`                                                 |
| Venue badge colours                    | `_data/venues.yml`                                                                |
| Research projects                      | `_projects/*.md` (one file per project; images in `assets/img/`)                  |
| News items                             | `_news/*.md` (one file per item)                                                  |
| CV page                                | `_data/cv.yml`                                                                    |
| CV PDF                                 | `assets/pdf/Sayumi_Muthukumarana_CV.pdf`                                          |
| Social and contact links               | `_data/socials.yml`                                                               |
| Site title, description, settings      | `_config.yml`                                                                     |

### Add a news item

Create `_news/2026-12-my-news.md`:

```markdown
---
layout: post
date: 2026-12-01 09:00:00+0530
inline: true
related_posts: false
---

Short announcement with a [link](https://example.com).
```

News shows the month and year. To show something else (for example just "2025"), add `display_date: "2025"` to the front matter.

### Add a publication

Add a BibTeX entry to `_bibliography/papers.bib`. Useful extra fields:

- `abbr = {MERCon}`: venue badge (colour and link set in `_data/venues.yml`)
- `selected = {true}`: also show it on the homepage
- `bibtex_show = {true}`: show the "Bib" button
- `arxiv = {2601.01234}`, `html = {https://...}`, `pdf = {https://...}`, `code = {https://...}`: link buttons
- `abstract = {...}`: the "Abs" button
- `note = {Under review at ...}`: status line
- `preview = {image.jpg}`: thumbnail from `assets/img/publication_preview/`

### Things to fill in

- **arXiv ID** for "Once Upon a Bias": add `arxiv = {XXXX.XXXXX}` to the entry `muthukumarana2026onceuponabias` in `_bibliography/papers.bib`.
- **Abstracts:** the "Abs" text for each paper is a summary taken from the CV. Replace it with the real paper abstracts when you can.
