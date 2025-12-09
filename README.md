# EPUB Professional Editor

[![GitHub release](https://img.shields.io/github/v/release/BR1JM0H4N/Epub-editor?style=flat-square)](https://github.com/BR1JM0H4N/Epub-editor/releases)
[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/BR1JM0H4N/Epub-editor/pages.yml?branch=main&style=flat-square&label=Pages%20Deploy)](https://github.com/BR1JM0H4N/Epub-editor/actions)
[![GitHub issues](https://img.shields.io/github/issues/BR1JM0H4N/Epub-editor?style=flat-square)](https://github.com/BR1JM0H4N/Epub-editor/issues)
[![License: MIT](https://img.shields.io/github/license/BR1JM0H4N/Epub-editor?style=flat-square)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/BR1JM0H4N/Epub-editor?style=flat-square)](https://github.com/BR1JM0H4N/Epub-editor/stargazers)

---

**Online Demo:**  
👉 [https://br1jm0h4n.github.io/Epub-editor/](https://br1jm0h4n.github.io/Epub-editor/)

---

## ✨ EPUB Professional Editor

A modern, privacy-first in-browser EPUB editor to modify eBooks — all processing is done client-side in your browser! 

Edit metadata, fix or replace covers, auto-generate tables of contents, and perform bulk find-and-replace operations across your EPUB files without uploading them to any server.

---

## Features

- **Android 15 dark theme**: Stylish, accessible UI.
- **Edit Metadata**: Change title, author, language, and publisher.
- **Cover Image Handling**:
  - Replace existing covers (auto-updates manifest and metadata).
  - Optionally generate or fix a proper cover page/front wrapper.
  - Ensure the cover is the first spine item for optimal reader display.
- **EPUB Table of Contents**:
  - Auto-generate or update NCX TOC from customizable CSS selectors (`h1`, `h2`, `.chapter-title` etc.).
  - Preview TOC structure before saving.
- **Bulk Find & Replace**:
  - Define multiple text/regex replacement rules.
  - Test transformations live with input/output preview.
  - Apply to all XHTML/HTML chapters at once.
- **Instant Download**: Click once to generate and download the modified EPUB.
- **Zero server-side code**: Privacy preserved—your book never leaves your device.
- **Mobile Friendly**: Usable on tablets and large-screen mobile browsers.

---

## Usage

1. **Open the editor:**  
   [https://br1jm0h4n.github.io/Epub-editor/](https://br1jm0h4n.github.io/Epub-editor/)
2. **Upload your EPUB** using the file picker.
3. Edit the **metadata** and/or **cover** as needed.
4. Optionally, use **Bulk Find & Replace** to clean up common OCR artifacts or text patterns.
5. Optionally, regenerate the **Table of Contents** using your own selectors.
6. Click **Generate & Download EPUB** to get the edited book.

_All changes are processed instantly in-browser. The original file is never uploaded._

---

## Screenshots

![Editor main UI](https://user-images.githubusercontent.com/BR1JM0H4N/Epub-editor/main/screenshot1.png)
![Find and Replace modal](https://user-images.githubusercontent.com/BR1JM0H4N/Epub-editor/main/screenshot2.png)

---

## Development

- Built with standard HTML, CSS (custom properties), and vanilla JavaScript.
- [JSZip](https://stuk.github.io/jszip/) is used for EPUB (ZIP) processing.
- Debug console powered by [eruda](https://github.com/liriliri/eruda) (visible on mobile).

### Run locally

Clone the repo and simply open `index.html` in your browser. No build tools required.

```sh
git clone https://github.com/BR1JM0H4N/Epub-editor.git
cd Epub-editor
open index.html   # or drag into browser
```

---

## License

MIT &copy; [BR1JM0H4N](https://github.com/BR1JM0H4N)

---

## Credits

- [JSZip](https://github.com/Stuk/jszip)
- [eruda](https://github.com/liriliri/eruda)
- Book and EPUB specification insights from [idpf.org](https://www.w3.org/publishing/epub3/epub-changes.html)

---

## Feedback & Issues

If you hit problems or have requests, file an [issue](https://github.com/BR1JM0H4N/Epub-editor/issues) or open a [discussion](https://github.com/BR1JM0H4N/Epub-editor/discussions).
