# PhD Thesis in LaTeX

This repository contains the LaTeX source files for my PhD thesis. The structure of the project allows for flexible compilation of different chapters and sections as needed.

## Repository Structure

```
📂 thesis/
├── 📄 main.tex                       # Main LaTeX file (select chapters to compile)
├── 📂 chapters/                      # Contains chapter subfolders
|   ├── 📄 chapter1.tex               # Chapter 1 file (select sections to compile)  
|   ├── 📄 chapter2.tex            
|   ├── 📄 chapter3.tex            
|   ├── 📄 ...            
│   ├── 📂 chapter1/                  # Chapter 1 folder
│   │   ├── conventionalDetection.tex  # Section file
│   │   ├── egfet.tex                 
│   │   ├── fet.tex                    
│   │   └── ...
│   ├── 📂 chapter2/                  # Chapter 2 folder
│   │   ├── characterization.tex       # Section file
│   │   ├── cntDeposition.tex         
│   │   └── ...
│   └── ...                            # Additional chapter folders
├── 📂 Figures/                        # Folder for figures
│   ├── 📂 chapter1/                   # Figures for Chapter 1
│   │   ├── 📂 conventionalDetection/  # Figures for section
│   │   ├── 📂 egfet/                  
│   │   ├── 📂 fet/                    
│   │   └── ...
│   ├── 📂 chapter2/         # Figures for Chapter 2
│   └── ...
├── 📄 macros.tex             # Contains custom macros used across files
├── 📄 preamble.sty           # Defines style and format of the document
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

Alternatively, use a LaTeX text editor.

## Customization

- **Chapters**: Include or exclude specific chapters by modifying `main.tex`.
- **Sections**: Chapters reference section files, which can be modified individually.
- **Figures**: Store and reference figures in their corresponding chapter and section folders.
- **Macros**: Define custom macros in `macros.tex` for easier LaTeX writing.
- **Preamble**: Modify `preamble.sty` to change the thesis formatting.

## Dependencies

Ensure you have the following installed:

- **TeX Live** or **MikTeX**
- **biber**
- **latexmk** (optional, for automated compilation)

## Contact

For any questions or contributions, feel free to open an issue or reach out to me.


