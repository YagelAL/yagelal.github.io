# Yagel Alfasi — Portfolio

A minimal, single-page portfolio site presenting coursework and independent
projects in statistics, machine learning, GIS, distributed systems, and applied
mathematics. No backend, no build step, no dependencies — just `index.html`,
plus the linked files under `assets/files/`.

Each card links out to that project's folder on GitHub or its repository.

## View it locally

Open `index.html` in a browser — everything is self-contained.

## Publish with GitHub Pages

1. Create a repository on GitHub, or use an existing one.
2. Push this folder's contents to the repo:
   ```bash
   cd portfolio-site
   git init
   git add .
   git commit -m "Add portfolio site"
   git branch -M main
   git remote add origin https://github.com/<username>/<repo-name>.git
   git push -u origin main
   ```
3. In the repo's **Settings → Pages**, set **Source** to "Deploy from a branch,"
   select the `main` branch and `/ (root)` folder, then save.
4. GitHub Pages will publish the site within a couple of minutes.

To update the site, edit `index.html` and push again — Pages redeploys
automatically on every push to `main`.

## Editing project entries

Each card is one object in the `MAIN_PROJECTS` or `SECONDARY_PROJECTS` array
inside `index.html`. Each entry has an `emoji`, a `title`, a one-line `desc`,
and an `href` (a relative `assets/files/...` path or a full URL).

## Editing publications

Each entry in the `PUBLICATIONS` array has a `label` (e.g. "Preprint · arXiv"),
a `title`, a `desc`, and an `href` linking to the paper.

## Folder structure

```
index.html        — the site (HTML, CSS, and JS in one file)
assets/files/      — project files and reports, organized by project
README.md         — this file
```
