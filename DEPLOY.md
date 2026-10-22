# Deployment Guide — Zhenghao Chen's Academic Homepage

This guide covers uploading this folder to GitHub and publishing it with GitHub Pages, plus how to keep the content up to date.

## 0. What you have

- A static, **markdown-driven** GitHub Pages site — there is no build step; the page fetches `contents/*.md` and renders them in the browser.
- **Bilingual** content: English (default) + 中文, switchable with the **EN / 中文** button in the navbar.
- GitHub username: **`Chris0829`** · repository: **`Chris0829.github.io`** · live site: **https://chris0829.github.io/**

## 1. Push the site

This folder is already a git repository with `origin` pointing at `https://github.com/Chris0829/Chris0829.github.io.git`.

```bash
# from inside this folder
git add -A
git commit -m "Deploy Zhenghao Chen's homepage (EN/中文 bilingual)"
git push -u origin main
```

## 2. Enable GitHub Pages

1. GitHub → repo **Chris0829/Chris0829.github.io** → **Settings** → **Pages** (left sidebar, under "Code and automation").
2. **Build and deployment → Source**: choose **Deploy from a branch**.
3. **Branch**: select `main`, folder **`/ (root)`** → **Save**.
4. Wait a few minutes (up to ~10 minutes for the first publish).

## 3. Verify

Open **https://chris0829.github.io/**

Check that: the navbar shows **HOME / NEWS / RESEARCH / PUBLICATIONS / AWARDS / SERVICE**; the **EN / 中文** toggle switches language; your photo and background images appear.

## 4. Updating content later

| What to change | Where |
| --- | --- |
| Name, tagline, nav, section titles | `contents/config.yml` (EN) and `contents/zh/config.yml` (中文) |
| English section text | `contents/home.md`, `news.md`, `research.md`, `publications.md`, `awards.md`, `service.md` |
| Chinese section text | `contents/zh/*.md` |
| Profile photo | replace `static/assets/img/photo.png` |
| Background images | replace `static/assets/background/background_0.jpeg` and `background_1.jpeg` (add more and list them in **both** `config.yml` files) |
| Google Scholar badge | edit the badge link in `contents/home.md` and `contents/zh/home.md` (currently a placeholder) |

After any change: `git add -A && git commit -m "update" && git push`.

## 5. Local preview (optional)

Because the page loads content via `fetch()`, opening `index.html` directly (`file://`) will not work — serve it over HTTP:

```bash
# Python 3, from inside this folder
python -m http.server 8000
# then open http://localhost:8000/
```

## 6. Files checklist (all present and used)

```
index.html                           # page shell: meta, nav, EN/中文 toggle, hero, footer
contents/config.yml                  # EN config (title, tagline, sections, backgrounds, links)
contents/zh/config.yml               # 中文 config
contents/{home,news,research,publications,awards,service}.md    # EN content
contents/zh/{home,news,research,publications,awards,service}.md # 中文 content
static/css/main.css                  # theme + custom styles (toggle, <details>, blockquote)
static/css/styles.css                # Bootstrap 5 + Start Bootstrap New Age
static/js/scripts.js                 # rendering engine (sections, markdown, language toggle, slideshow)
static/js/{marked,js-yaml,bootstrap.bundle.min,tex-svg}.min.js # third-party libs
static/assets/img/photo.png          # profile photo (replace with your real photo)
static/assets/background/*.jpeg      # slideshow backgrounds
static/assets/favicon.ico            # favicon
LICENSE                              # MIT (template attribution — keep)
tests/*.test.js                      # quality checks (Node.js; optional)
screenshot_full.png                  # template screenshot (can delete or replace)
```

## 7. License / attribution

Built on [academic-homepage-template](https://github.com/senli1073/academic-homepage-template) by Sen Li (MIT). Please keep the `LICENSE` file in place.
