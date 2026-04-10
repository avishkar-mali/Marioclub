# Repository Guidelines

## Project Structure & Module Organization
This repository is a small static site. The main page lives in `index.html`, and all styling is in `styles3.css`. Image assets are stored at the repository root as `mario.jpg`, `gamenew02.jpg`, and `gamenew3.jpg`. Keep new assets lightweight and use descriptive names such as `event-banner.jpg` or `tournament-card.png`. `README.md` contains the public project link; update it when deployment details change.

## Build, Test, and Development Commands
There is no build step or package manager in this project.

- `start index.html`
  Opens the site locally in the default browser on Windows.
- `python -m http.server 8000`
  Runs a simple local server for checking links, images, and form layout at `http://localhost:8000`.
- `git status`
  Review pending changes before committing.

## Coding Style & Naming Conventions
Use 2-space indentation in HTML and keep markup semantic with clear landmarks such as `header`, `main`, `section`, and `footer`. In CSS, prefer custom properties in `:root` for shared colors and spacing. Reuse existing class patterns like `.feature-card`, `.join-form`, and `.checkbox-row` instead of adding one-off selectors. Use lowercase, hyphenated names for classes and IDs.

## Testing Guidelines
Testing is currently manual. Before opening a pull request, verify the page in a desktop browser and a narrow mobile viewport. Confirm that navigation anchors scroll correctly, images load, and the join form remains readable and usable. If you change copy, double-check text encoding and punctuation in the browser.

## Commit & Pull Request Guidelines
Recent commits use short, imperative summaries such as `Enhance homepage UI with richer layout and join form` and `For Mobile`. Prefer clearer versions of that style, for example `Improve mobile spacing in join form`. Keep each commit focused on one change. Pull requests should include a short description, note any visual or responsive changes, and attach screenshots for UI updates.

## Content & Asset Notes
Do not introduce large binary files without need. Optimize new images before committing, and keep references relative, for example `./assets/hero.jpg` if an asset folder is added later.
