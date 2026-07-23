# CODA ISMIR 2026 Manuscript

This repository contains the camera-ready manuscript source for:

> CODA: Cascaded Online Discontinuity-Aware Alignment for Real-Time Image-Based Score Following

## Repository layout

- `main.tex` - preamble, title, authors, abstract, section includes, and bibliography
- `sections/` - one file per major manuscript section
- `figures/` - manuscript figures
- `references.bib` - bibliography database
- `ismir.sty`, `cite.sty`, `IEEEtran.bst`, `cc_by.pdf` - files required by the ISMIR template
- `template/ISMIR_2026_Paper_Template/` - untouched official ISMIR 2026 template reference
- `reviews/` - formal reviews, meta-review, camera-ready instructions, and internal review material
- `notes/` - revision and reference-audit working notes that are not part of the paper build

## Build

From the repository root:

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex
```

The final manuscript is written to `main.pdf`. To remove intermediate LaTeX files while keeping the PDF:

```sh
latexmk -c main.tex
```

## Template integrity

The root `ismir.sty` must remain byte-for-byte identical to:

`template/ISMIR_2026_Paper_Template/latex/ismir.sty`

Do not edit or override the official style file.

