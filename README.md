# Dr. Vimal Kumar — academic website

Personal academic website built on the [al-folio](https://github.com/alshedivat/al-folio) Jekyll template (v1.x).

**Live URL (after the first deploy):** https://gkkumargaurav2-beep.github.io/VKumar/

## Pages

| Page            | File                                                  | What it shows                                                       |
| --------------- | ----------------------------------------------------- | ------------------------------------------------------------------- |
| about (home)    | `_pages/about.md`                                     | Bio, headline numbers, news, selected publications, profile links   |
| research        | `_pages/research.md`                                  | Four research themes with key papers; projects                      |
| publications    | `_pages/publications.md` + `_bibliography/papers.bib` | 247 entries grouped by ABDC rank, chapters, conferences; searchable |
| teaching        | `_pages/teaching.md`                                  | Course summary tables                                               |
| students        | `_pages/students.md`                                  | PhD and Master's supervision; prospective students                  |
| talks & service | `_pages/service.md`                                   | Editorial roles, invited talks, session chairs, awards              |
| CV              | `_pages/cv.md` + `_data/cv.yml`                       | Short public CV                                                     |

## First-time setup on GitHub (one time only)

1. **Settings → Actions → General → Workflow permissions:** choose **Read and write permissions** and save. The deploy workflow needs this to publish.
2. Push these files to the `main` branch. The **Deploy site** workflow (Actions tab) builds the site and writes it to the `gh-pages` branch. Wait for the green tick (about 5–8 minutes).
3. **Settings → Pages → Build and deployment:** Source = **Deploy from a branch**, Branch = **gh-pages**, folder **/ (root)**. Save.
4. Open https://gkkumargaurav2-beep.github.io/VKumar/ a minute later.

If the page loads without styling, check that `url` and `baseurl` in `_config.yml` are `https://gkkumargaurav2-beep.github.io` and `/VKumar`.

### Using a custom domain later

Add a `CNAME` file containing the domain (e.g. `vimalkumar.com`), set `url: https://vimalkumar.com` and `baseurl:` (empty) in `_config.yml`, then add the domain under Settings → Pages.

## Routine updates

- **New paper:** add an entry to `_bibliography/papers.bib`. Set `abbr` to `ABDC A`, `ABDC B`, `ABDC C`, `Journal`, `Chapter` or `Conference`, and `tier` to `a`, `b`, `c`, `other`, `chapter` or `conference` so it lands in the right section. Add `selected = {true}` to feature it on the home page.
- **News:** add a short file to `_news/` (copy an existing one and change the date and text). Remove old items once or twice a year.
- **Photo:** replace `assets/img/prof_pic.jpg` (keep the file name; about 800 px wide JPEG works well). The current one is the formal suit portrait, 800 × 1029 px.
- **CV download:** put a public-safe PDF at `assets/pdf/Vimal_Kumar_CV.pdf` and uncomment `cv_pdf` in `_data/socials.yml`. Do not publish the full CV with date of birth, family details, home addresses or phone numbers.

See `CONTENT-NOTES.md` for items in the CV data that still need checking.
