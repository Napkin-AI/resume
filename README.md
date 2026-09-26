# Resume

This repository contains the source files and compiled PDF versions of my resume in **English** and **Russian**.

The resume is written in **LaTeX** and is based on [Jake's Resume](https://www.overleaf.com/latex/templates/jakes-resume/syzfjbzwjncs)

## Files

```text
.
├── resume_mironov_arseniy_en.tex        # English LaTeX source
├── resume_mironov_arseniy_en.pdf        # English resume
├── resume_mironov_arseniy_ru.tex        # Russian LaTeX source
├── resume_mironov_arseniy_ru.pdf        # Russian resume
└── README.md                            # This file

```

## Build

The project can be built directly from VS Code using the [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) extension.

Using `latexmk`:

```bash
latexmk -pdf -outdir=. -auxdir=build resume_mironov_arseniy_en.tex
latexmk -pdf -outdir=. -auxdir=build resume_mironov_arseniy_ru.tex
```

Or using `pdflatex` directly:

```bash
pdflatex -interaction=nonstopmode -halt-on-error resume_mironov_arseniy_en.tex
pdflatex -interaction=nonstopmode -halt-on-error resume_mironov_arseniy_ru.tex
```
