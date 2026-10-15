# carl-h.com

Source for my personal website, [carl-h.com](https://carl-h.com). It is a single-page CV built with [Jekyll](https://jekyllrb.com/) and hosted on GitHub Pages.

## Running it locally (Ubuntu)

Install Ruby and the build tools (one time):

```bash
sudo apt install ruby-full build-essential zlib1g-dev
```

Install the gems (one time, and again whenever the `Gemfile` changes):

```bash
bundle install
```

If `bundle` isn't found, install it with `sudo gem install bundler`. The gems go into `vendor/bundle` inside this folder, as set in `.bundle/config`, so nothing is installed system-wide.

Start the site:

```bash
bundle exec jekyll serve --livereload
```

Then open <http://localhost:4000>. The page reloads automatically when you save a file. Changes to `_config.yml` need a restart.

## Deploying

Push to `master` and GitHub Pages rebuilds the live site automatically. The `github-pages` gem in the `Gemfile` uses the same Jekyll version and plugins as GitHub Pages, so what you see locally is what goes live.

## Editing content

Almost everything is data. You shouldn't need to touch the HTML.

| What | Where |
| --- | --- |
| Name, bio, contact, social links, CV link | `_data/profile.yml` (top) |
| Experience, education, awards, teaching, service | `_data/profile.yml` (lists, shown in that order) |
| Publications | `_publications/` (one file per paper) |
| Patents | `_patents/` (one file per patent) |
| PDFs (papers, slides, posters, CV) | `assets/files/` |
| Company and school logos | `assets/images/logos/` |

### Adding a publication

Create `_publications/YYYY-MM-DD-short-name.md`. Only these fields are shown on the site:

```yaml
---
title: "Paper Title"
author: [First Author, Carl Hildebrandt, Last Author]
venue: "International Conference on Software Engineering (ICSE)"
year: 2025
date: 2025-05-27
downloads:
  paper: /assets/files/publications/ICSE25-Short.pdf
  slides: /assets/files/slides/ICSE25-Short-Slides.pdf
  artifact: https://github.com/...
citation: "First Author, Carl Hildebrandt, Last Author. 2025. Paper Title. In <i>Booktitle</i>. 1-10. https://doi.org/..."
---
```

- `date` sets the order (newest first).
- The text in brackets at the end of `venue` becomes the tag (e.g. "ICSE 2025"). To use a different tag, set `venue_short: "ICSE-NIER"`.
- `downloads` can use any labels. Each one becomes a button.
- `citation` is only used in the printed version of the page.
- Extra fields such as `abstract`, `doi` and `booktitle` are fine to keep for your own records. The site just doesn't display them.

### Adding a patent

Copy one of the files in `_patents/`. Patents work like publications but use `patent_number` instead of `venue`.

### Logos

Set `logo: name.png` on a position or education entry and put the image in `assets/images/logos/`. Logos sit on a white tile. For a transparent logo that should sit directly on the page, also set `logo_plain: true`. If there is no logo, the first letter is shown instead.

### Printing

Printing the page (Ctrl+P) gives a plain CV. Cards, photos and buttons are hidden, and publications are listed by their `citation`.

## Project layout

```
_config.yml          Site settings
_data/profile.yml    All CV content except publications and patents
_publications/       One file per paper
_patents/            One file per patent
_layouts/cv.html     The page itself (also holds the light/dark toggle script)
_includes/           One file per CV section, plus small shared pieces
_sass/               Styles: colours (variables), base, cv, icons
assets/css/style.scss  Combines the _sass files into style.css
assets/fonts/        Icon font (see the README there to add icons)
```

This site is based on [David Shriver's website](https://dlshriver.com/).
