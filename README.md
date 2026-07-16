# Talking Book Builder

A standalone, offline-capable web application for documenting indigenous and endangered languages through recorded audio, photography, and transcription. Built for fieldwork linguists, language community members, and students.

Available in **English** (`talking_book.html`) and **Spanish / Español** (`talking_book_es.html`).

---

## What it does

Talking Book Builder helps you create printable, audio-linked storybooks from language documentation materials. Each book has a cover page and a sequence of story pages, each containing an illustration, a transcription, and a QR code (on the cover) linking to a cloud-hosted audio recording.

### Key features

- **Story page editor** — add pages with transcription text and illustrations (.jpg / .png)
- **ELAN .eaf import** — select a tier and every annotation becomes a page, ordered by start time
- **Cloud audio link** — paste a Google Drive, Dropbox, or YouTube URL; a QR code is generated automatically for the printed cover
- **Print-ready output** — full-bleed cover with title, speaker, artist, project team, and QR code; one page per story page with image above text
- **Auto font scaling** — optional: font size shrinks to fit text on a single page if needed; configurable font family and base size
- **Markdown export** — YAML front matter with all metadata, embedded base64 images, and a QR code rendered as an image
- **Project save / load** — JSON archive preserves all text, images, and settings across sessions
- **Merge projects** — combine JSON files from multiple contributors with conflict resolution
- **New Book** — clear the workspace and start fresh

---

## How to use

1. Download `talking_book.html` (English) or `talking_book_es.html` (Spanish)
2. Open the file in any modern browser — no installation, no internet required
3. Fill in the story details in the left sidebar
4. Add pages manually or import annotations from an ELAN `.eaf` file
5. Upload an illustration for each page
6. Paste a cloud audio link to generate the cover QR code
7. Click **Print book** to produce a school-ready PDF via your browser's print dialog
8. Click **Export Markdown** for a self-contained `.md` file for further processing
9. Click **Save project (JSON)** to preserve your work

### Collaborative workflow

The app is designed for offline fieldwork. For multi-person projects:

1. The editor shares the master JSON with contributors
2. Each contributor loads it, works on their assigned pages, and saves their own copy
3. The editor uses **Merge project (JSON)** to combine all contributions, resolving any page-level conflicts in a dialog

---

## Files

| File | Description |
|---|---|
| `talking_book.html` | English version |
| `talking_book_es.html` | Spanish / Español version |
| `README.md` | This file |

---

## Fonts

The printed book uses **Noto Sans** by default (loaded from Google Fonts when online). Noto Sans has excellent Unicode coverage for indigenous language characters and diacritics. When offline, the browser falls back to system fonts (Segoe UI on Windows, Helvetica Neue on Mac/iOS, Noto Sans on Android).

For fully offline Noto Sans: download `NotoSans-Regular.woff2` and `NotoSans-SemiBold.woff2` from [fonts.google.com](https://fonts.google.com/noto/specimen/Noto+Sans), place them in the same folder as the HTML file, and uncomment the `@font-face` blocks in the CSS.

---

## Citation

If you use Talking Book Builder in your research or language documentation work, please cite it as:

> Rogers, Chris. 2025. *Talking Book Builder*. Software.

---

## License

© 2025 Chris Rogers

This software is made available for **individual, non-commercial use only**.

### Permitted use

- A student, researcher, or community member using the tool for personal or academic language documentation

### Not permitted without a license

- Commercial use of any kind
- Deployment or distribution for use by a group, organization, institution, or classroom

### Licensing

For institutional, classroom, or commercial licensing inquiries, contact:
**chris.linguist@gmail.com**

All rights reserved. Unauthorized commercial use or group deployment of this software is prohibited.

---

## About

Talking Book Builder is part of the language documentation toolkit at [languageconservation.org](https://languageconservation.org), supporting the documentation and revitalization of indigenous and endangered languages.
