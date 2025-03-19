# PhD Thesis in LaTeX

This repository contains the LaTeX source files for my PhD thesis. The structure of the project allows for flexible compilation of different chapters and sections as needed.

## Repository Structure

```
📂 thesis/
├── 📄 main.tex               # Main LaTeX file (selects chapters to compile)
├── 📂 chapters/              # Contains individual chapter files
│   ├── chapter1.tex         # Chapter 1 file (includes sections)
│   ├── chapter2.tex         # Chapter 2 file
│   └── ...                  # Additional chapter files
├── 📂 sections/              # Contains individual section files
│   ├── section1_1.tex       # Section 1.1 file
│   ├── section1_2.tex       # Section 1.2 file
│   └── ...                  # Additional sections
├── 📂 figures/               # Folder for figures
│   ├── 📂 chapter1/         # Figures for Chapter 1
│   │   ├── 📂 section1_1/   # Figures for Section 1.1
│   │   ├── 📂 section1_2/   # Figures for Section 1.2
│   │   └── ...
│   ├── 📂 chapter2/         # Figures for Chapter 2
│   └── ...
└── 📄 bibliography.bib       # Bibliography file
```

## Compilation Instructions

To compile the thesis, use the following command:

```bash
pdflatex main.tex
biber main      # If using BibLaTeX
pdflatex main.tex
pdflatex main.tex
```

Alternatively, use a LaTeX text editor

## Customization

- **Chapters**: Include or exclude specific chapters by modifying `main.tex`.
- **Sections**: Chapters reference section files, which can be modified individually.
- **Figures**: Store and reference figures in their corresponding chapter and section folders.

## Dependencies

Ensure you have the following installed:

- **TeX Live** or **MikTeX**
- **biber** (if using BibLaTeX for references)
- **latexmk** (optional, for automated compilation)

## Contact

For any questions or contributions, feel free to open an issue or reach out to me.


