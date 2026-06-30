# Personal website — Jonathan E. Prunty

Source for my personal academic site, built with [Jekyll](https://jekyllrb.com/)
and hosted on GitHub Pages. Most content is data-driven, so day-to-day updates
mean editing a few lines of YAML — no HTML required.

## Where things live

| What you want to change            | File                       |
| ---------------------------------- | -------------------------- |
| Name, role, bio, social links, CV  | `_config.yml`              |
| News items                         | `_data/news.yml`           |
| Publications                       | `_data/publications.yml`   |
| Colours, fonts, spacing            | `assets/css/main.css`      |
| Page structure / layout            | `index.html`, `_layouts/default.html` |
| Profile photo                      | `images/profilePic.png`    |

### Add a news item
Open `_data/news.yml` and copy a block to the top:

```yaml
- date: Jun 2026
  content: >-
    Short update. **Markdown** and *italics* work here.
```

### Add a publication
Open `_data/publications.yml` and copy a block to the top. Leave any link blank
to hide it:

```yaml
- title: "Paper title"
  authors: "A. Author, **J. E. Prunty**, B. Author"
  venue: "Journal Name"
  year: 2026
  links:
    doi: https://doi.org/...
    pdf: /pdf/yourpaper.pdf
    code: https://github.com/...
```

### Recolour the site
Edit the variables at the top of `assets/css/main.css` (e.g. `--accent`).
A light and dark palette are defined; visitors get a toggle in the corner.

## Preview locally (optional)

Requires Ruby. Then:

```bash
bundle install
bundle exec jekyll serve
```

Open <http://localhost:4000>. Otherwise just push to `main` and GitHub Pages
will build it automatically.

---

Originally forked from a minimal portfolio template; since rebuilt.
