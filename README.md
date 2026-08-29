# One-column research paper template

This repository is a clean, modular LaTeX starting point for a technical paper.
All numerical results and scientific claims are dummy content.

## Compile in VS Code

1. Open this `milestone` folder in VS Code.
2. Open `main.tex`.
3. Save the file or run **LaTeX Workshop: Build LaTeX project**.
4. Open `build/main.pdf` using **LaTeX Workshop: View LaTeX PDF**.

The included settings use `latexmk`, which automatically runs BibTeX and the
required additional LaTeX passes.

## Compile in a terminal

Compile the manuscript (the example figures are generated directly from their
TikZ/PGFPlots source):

```bash
latexmk -pdf -outdir=build main.tex
```

## Structure

- `main.tex`: paper entry point and packages
- `sections/`: individually editable paper sections
- `tables/`: reusable table fragments
- `figures/`: editable TikZ/PGFPlots figure source files
- `references.bib`: BibTeX references
- `.vscode/settings.json`: LaTeX Workshop configuration

To use this at `C:\Users\jiazh\OneDrive - Monash University\Desktop\milestone`,
extract or copy the repository into that location, then open the folder itself
in VS Code.
