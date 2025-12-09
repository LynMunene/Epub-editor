# Epub-editor

[![Demo](https://img.shields.io/badge/demo-GitHub%20Pages-blue?logo=github)](https://br1jm0h4n.github.io/Epub-editor/)
[![Pages build status](https://img.shields.io/github/pages/build/BR1JM0H4N/Epub-editor)](https://github.com/BR1JM0H4N/Epub-editor/actions?query=workflow%3A%22GitHub+Pages%22)
[![GitHub Actions](https://github.com/BR1JM0H4N/Epub-editor/actions/workflows/ci.yml/badge.svg)](https://github.com/BR1JM0H4N/Epub-editor/actions)
[![Last commit](https://img.shields.io/github/last-commit/BR1JM0H4N/Epub-editor)](https://github.com/BR1JM0H4N/Epub-editor/commits/main)
[![License](https://img.shields.io/github/license/BR1JM0H4N/Epub-editor)](https://github.com/BR1JM0H4N/Epub-editor/blob/main/LICENSE)
[![Stars](https://img.shields.io/github/stars/BR1JM0H4N/Epub-editor?style=social)](https://github.com/BR1JM0H4N/Epub-editor/stargazers)
[![Forks](https://img.shields.io/github/forks/BR1JM0H4N/Epub-editor?style=social)](https://github.com/BR1JM0H4N/Epub-editor/network/members)
[![Open issues](https://img.shields.io/github/issues/BR1JM0H4N/Epub-editor)](https://github.com/BR1JM0H4N/Epub-editor/issues)
[![Top language](https://img.shields.io/github/languages/top/BR1JM0H4N/Epub-editor)](https://github.com/BR1JM0H4N/Epub-editor)

A lightweight, browser-first EPUB editor and toolkit — edit, preview and export EPUB files directly in your browser.

Live demo: https://br1jm0h4n.github.io/Epub-editor/

---

Table of contents
- [Demo](#demo)
- [Features](#features)
- [Screenshots / Demo GIF](#screenshots--demo-gif)
- [Quick start](#quick-start)
- [Usage](#usage)
- [Development](#development)
- [Build & Deploy (GitHub Pages)](#build--deploy-github-pages)
- [Contributing](#contributing)
- [License](#license)
- [Maintainers & Contact](#maintainers--contact)

Demo
----
Open the hosted demo: https://br1jm0h4n.github.io/Epub-editor/

Features
--------
- Edit EPUB content (HTML/CSS) in the browser
- Live preview of EPUB pages and layout
- Import and export .epub files (pack/unpack)
- Edit metadata (title, author, language) and table of contents
- Manage assets (images, fonts, CSS)
- WYSIWYG and source (HTML) editing modes
- Small, dependency-light codebase optimized for the web

Screenshots / Demo GIF
----------------------
Add a screenshot or short demo GIF to highlight the editor in action.

Suggested path: docs/demo.gif or assets/demo.gif

Example:
![Demo GIF](docs/demo.gif)

Quick start
-----------
Clone the repository and run the project locally.

```bash
git clone https://github.com/BR1JM0H4N/Epub-editor.git
cd Epub-editor
```

Install (example commands — adapt to the project's stack)
```bash
# npm
npm install

# or yarn
yarn install
```

Run in development mode
```bash
npm run dev
# or
yarn dev
```

Build for production
```bash
npm run build
# preview
npm run preview
```

If this project uses a different framework (e.g. Electron, Python backend), replace the above with the appropriate commands. If you're unsure, check package.json or the project docs for exact scripts.

Usage
-----
- Open the app in your browser (e.g., http://localhost:3000)
- Create a new book or import an existing .epub file
- Edit chapters using the editor or switch to source mode
- Add/remove assets (images, fonts, CSS)
- Edit metadata and table of contents
- Export or download the finished EPUB

Development
-----------
- Keep the code modular and testable.
- Prefer vanilla/tiny dependencies where possible to keep the build small.
- If adding features that increase bundle size, explain trade-offs in the PR description.

Common developer scripts (example)
```json
{
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "preview": "vite preview",
    "lint": "eslint .",
    "test": "vitest"
  }
}
```

Build & Deploy (GitHub Pages)
-----------------------------
The demo is hosted at https://br1jm0h4n.github.io/Epub-editor/

Recommended workflow:
- Build the project to a static output folder (often `dist/` or `docs/`).
- Push the built output to the `gh-pages` branch or enable GitHub Pages to serve from `main` / `docs`.
- Confirm the Pages build status and fix any asset/path issues (especially if your app uses client-side routing — configure base path).

Example: deploy to docs/ on main
```bash
npm run build
# move or copy build output to docs/ then push to main
```

Contributing
------------
Thank you for considering contributing!

- File an issue for bugs or feature requests.
- Fork the repository and create a feature branch.
- Add or update tests where applicable.
- Open a pull request with a clear description and link to related issues.

Code style
- Follow the project's linting rules.
- Keep changes small and focused (one feature/bug per PR).
- Ensure that the README, changelog, and docs are updated for user-facing changes.

License
-------
See the LICENSE file in this repository. If there is no license yet, add one (MIT is a common choice) and update the badge accordingly.

Maintainers & Contact
---------------------
- Maintainer: BR1JM0H4N
- GitHub: https://github.com/BR1JM0H4N

Roadmap (ideas)
---------------
- Improved WYSIWYG editing controls
- Plugin system for import/export transformations
- Better accessibility and keyboard controls
- EPUB 3 media overlays and interactivity support

Troubleshooting
---------------
- If EPUB import fails, verify the file is a valid .epub (ZIP container with mimetype and proper structure).
- If preview assets are missing, check that images/fonts were added to the package and referenced correctly.
- If GitHub Pages shows 404, confirm the base path is set correctly in app config (e.g., homepage or base for bundlers).

Notes for repository owners
---------------------------
- To showcase the app, add a short demo GIF to `docs/demo.gif` and ensure Pages serves the `docs/` folder (or build to `gh-pages` branch).
- If you want, I can prepare a PR that:
  - Adds this README.md to the repository.
  - Adds a small demo GIF placeholder and updates package.json scripts (if you provide the stack details).

Acknowledgements
----------------
- shields.io — for badges and simple status icons
- Inspiration from other web-based ebook editors and readers
