# ML Lessons Repository Guidelines

## Build Commands
- Compile LaTeX document: `pdflatex filename.tex`
- Compile with bibliography: `pdflatex filename.tex && bibtex filename && pdflatex filename.tex && pdflatex filename.tex`
- Clean auxiliary files: `rm -f *.aux *.log *.out *.toc *.bbl *.blg *.synctex.gz`

## Style Guidelines

### LaTeX Conventions
- Use `\documentclass{article}` for lessons, `\documentclass{beamer}` for slides
- Include standard packages: `\usepackage[utf8]{inputenc} \usepackage{amsmath,amssymb}`
- Maintain 1-inch margins with `\usepackage{geometry} \geometry{margin=1in}`
- Organize content with `\section*{}`, `\subsection*{}`, `\paragraph{}`

### Mathematical Notation
- Use `\mathcal{L}` for likelihood functions
- Use `J_{\text{MSE}}` format for cost functions with descriptive subscripts
- Wrap mathematical expressions in `\[ \]` for displayed equations
- Use `\Bigl( \Bigr)` for properly sized parentheses in equations

### File Organization
- Store lesson materials by topic in numbered directories (e.g., `lesson1/`)
- Follow naming convention: `lesson<number>.<part>.tex` for documents
- Use `slides<number>.<part>.tex` for presentation files
- Slides and lessons should cover the same material, without gaps. If asked to add something to the lesson, then also the slides should include that change, and vice-versa
- After every change do a git commit