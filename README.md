# rakhymzhan11.github.io

Personal academic website of Rakhymzhan Kazbek, built with [Zola](https://getzola.org)
and published to GitHub Pages by the workflow in `.github/workflows/build.yml`.

Live at <https://rakhymzhan11.github.io>.

## Layout

```
config.toml                  site title, base URL, and the nav menu
content/
  _index.md                  About (landing page)
  pubs.md                    Publications
  talks.md                   Talks and visiting positions
  teaching.md                Teaching
templates/
  base.html                  shared shell: <head>, site title, nav, footer
  index.html                 renders the landing section, plus Person JSON-LD
  page.html                  renders a normal page
  404.html
static/assets/
  main.css                   all styling
  main.js                    nav highlighting and KaTeX math rendering
```

## Local preview

Install Zola once:

```shell
brew install zola
```

Then, from this directory:

```shell
./serve
```

and open <http://127.0.0.1:1111>. The page reloads as you edit.

## Editing

* **Text** — edit the Markdown in `content/`. The `+++ ... +++` block at the top is
  the front matter; leave `title` and `template` in place.
* **Nav menu** — edit the `menu` list in `config.toml`. Adding a page means creating
  `content/<name>.md` and adding a matching `{ name = "...", url = "/<name>/" }` entry.
* **Styling** — `static/assets/main.css`.
* **Photo** — the landing page expects a headshot at `static/assets/images/photo.jpg`.
  `./add-photo <file>` converts and renames any image into place, and `./add-photo`
  with no arguments takes it from the clipboard. It is cropped to a 180px circle, so
  anything roughly square or portrait works. If the file is missing the image hides
  itself rather than showing a broken icon.
* **Math** — write LaTeX between `$...$` (inline) or `$$...$$` (display); KaTeX renders
  it in the browser.

## Publishing

Push to `main`. The GitHub Action installs Zola, runs `zola build`, and deploys
`public/` to GitHub Pages. Watch it under the repository's **Actions** tab.

The Pages source must be set to **GitHub Actions** (Settings → Pages → Build and
deployment → Source), not "Deploy from a branch".

## Custom domain

Put the domain in `static/CNAME` (one line, no scheme), change `base_url` in
`config.toml` to match, and add the domain under Settings → Pages → Custom domain.
