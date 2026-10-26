# Andrew Honer — Engineering Portfolio

Mechanical engineering portfolio for Andrew Honer.

## Edit the site

- Edit `content.json` for the homepage introduction, project descriptions, facts, captions, and galleries.
- Edit `pages.json` for About, Contact, and homepage About text. The About photo filename, alt text, and caption are in its `about` object.
- Put optimized website images in `dist/assets/`. Keep descriptive filenames and update matching image references and alt text.
- Replace `dist/assets/Andrew_Honer_Resume.pdf` when updating the Resume. Resume highlights are in `build.py`.
- Run `python3 build.py`, review the result, and commit the changed source and generated pages.

## Preview

Open `dist/index.html` in a browser, or run `python3 -m http.server 8000 --directory dist`.

## Deploy

The GitHub Actions workflow builds the site using Python’s standard library and deploys only `dist/` to GitHub Pages. Choose GitHub Actions as the Pages source. A push to `main` or a manual workflow run deploys an update.

## Add a project

Copy a project object in `content.json`, give it a unique slug and project number, and replace its content. Add suitable website images to `dist/assets/`, then rebuild. The Projects page updates automatically. Homepage featured projects are the first two items; later items appear in the ongoing-work list.

This repository contains only the website, its editable content and build code, optimized website images, and the public Resume.
