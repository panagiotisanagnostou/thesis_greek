# Thesis LaTeX Project

This repository contains the LaTeX source for a thesis/document. Build the PDF from `main.tex`.

## Repository structure

- `main.tex` — main document that includes chapters
- `1intro.tex`, `2relworks.tex`, `6sourcecode.tex` — chapter/source files
- `abstract.tex`, `acknowledgements.tex` — front/back matter
- `references.bib` — bibliography database
- `hellas.bst` — bibliography style file
- `figures/` — folder containing image assets

## Requirements

- A TeX distribution (TeX Live, MiKTeX, etc.)
- `bibtex` for bibliography processing (or `biber` if you adapt the workflow)

## Quick build (pdflatex + bibtex)

Run these commands from the project root:

```sh
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Alternatively, if you prefer XeLaTeX:

```sh
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

## Notes

- Add figures to the `figures/` folder and reference them from chapter files.
- Edit chapter files directly; `main.tex` assembles the final document.

If you'd like, I can add a `Makefile` or build script for one-command compilation.
