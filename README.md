# Haider Ghanem · CV

Personal CV site of **Haider Ghanem (حيدر غانم)**, full-stack engineer in Baghdad, Iraq.

**Live:** https://h19kod.github.io/my_cv/ · **Arabic:** https://h19kod.github.io/my_cv/?lang=ar

## What's inside

- **One file, no build step.** `index.html` holds the markup, styles and scripts. No framework and no dependencies beyond Google Fonts.
- **English and Arabic.** A full right-to-left Arabic version, switched from the toolbar or with `?lang=ar`.
- **Day and night modes.** Follows the system setting, and remembers the visitor's choice.
- **Command menu.** Press `Ctrl K` (or `⌘K`, or `/`) to jump to a section, open a project, copy the email or change the theme.
- **Live GitHub numbers.** Repository count, last push and main languages, fetched from the GitHub API.
- **Motion.** A 3D portrait that follows the pointer, gold dust, scroll reveals. All of it switches off for visitors who prefer reduced motion.
- **Ishtar Gate dividers.** Glazed-brick bands with rosettes and a small winged lion between sections.
- **Architecture diagram.** The Smart Ordering project opens an interactive diagram: hover or tap a part to see what it does.
- **A hidden piano.** Type `piano` anywhere (or click the piano icon next to PIANOVA) and play one octave with the keys A to K.
- **Print-ready.** Printing gives a clean two-page CV with a QR code to the live site. A plain-text version for applicant tracking systems is also included.

## Files

| File | Purpose |
|---|---|
| `index.html` | The site |
| `cv-plain.html` | Source of the plain-text (ATS) CV |
| `Haider_Ghanem_CV.pdf` | Designed CV, printed from `index.html` |
| `Haider_Ghanem_CV_ATS.pdf` | Plain-text CV, printed from `cv-plain.html` |
| `assets/haider.webp`, `assets/haider.jpg` | Portrait (WebP with JPEG fallback) |
| `assets/og.png` | 1200×630 preview image for link sharing |

## Run locally

```bash
python3 -m http.server 5500
```

Then open http://localhost:5500.

## Regenerate the PDFs

With the local server running, print each page to PDF from Chrome (Save as PDF, no headers and footers), or headless:

```bash
google-chrome --headless --no-pdf-header-footer --virtual-time-budget=6000 --print-to-pdf=Haider_Ghanem_CV.pdf http://localhost:5500/
google-chrome --headless --no-pdf-header-footer --print-to-pdf=Haider_Ghanem_CV_ATS.pdf http://localhost:5500/cv-plain.html
```

## Deploy

GitHub Pages: **Settings → Pages → Source: Deploy from a branch → `main` / root**.
