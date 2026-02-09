# Claude Instructions for DeepQuark Slides Project

## Project Overview

This project contains Beamer presentation slides for the paper "DeepQuark: Deep-Neural-Network Approach to Multiquark Bound States" (arXiv:2506.20555). The presentation is designed for a 25+5 minute talk at a hadron physics workshop.

## Key Files

- `slides.tex` - Main Beamer source file
- `arXiv-2506.20555v1/main.tex` - Original paper source (reference for content)
- `arXiv-2506.20555v1/*.pdf` - Figures from the paper

## Available Figures

| Figure | Content | Used in |
|--------|---------|---------|
| `framework.pdf` | DeepQuark architecture diagram | Slide 9 |
| `Graph_multiquark.pdf` | 2x2 convergence plots (a-d) | Slide 13 |
| `qqqFT.pdf` | Pairwise vs flux-tube confinement | Slide 13 |

## When Editing Slides

### Content Source
Always refer to `arXiv-2506.20555v1/main.tex` for:
- Exact equations and notation
- Numerical results (binding energies, radii, percentages)
- Parameter values from tables
- Author names and affiliations

### Key Results to Preserve
- Tcc: -15 MeV binding, 55%:45% color mixing, molecular structure
- Tbb: -153 MeV binding, 97% χ₃̄×₃, compact diquark (0.33 fm)
- T4c/T4b: No bound states
- Pentaquark S=5/2: P_ccbar(5715) at -3 MeV, P_bbbar(15569) at -14 MeV

### TikZ Diagrams
The slides use custom TikZ diagrams for:
- Molecular vs compact tetraquark structures
- VMC optimization loop
- Neural network architecture
- Pentaquark structure

Color scheme:
- `heavyblue` (RGB 0,70,140): Heavy quarks (c, b)
- `lightquarkorange` (RGB 230,120,50): Light quarks (u, d)

### Beamer Theme
- Theme: Madrid
- Aspect ratio: 16:9
- No navigation symbols
- Frame numbers in footer

## Building

```bash
pdflatex slides.tex
pdflatex slides.tex  # Second pass for references
open slides.pdf      # View on macOS
```

## Common Tasks

### Adding a new slide
```latex
\begin{frame}{Title}
\begin{columns}[T]
\begin{column}{0.48\textwidth}
% Left content
\end{column}
\begin{column}{0.48\textwidth}
% Right content
\end{column}
\end{columns}
\end{frame}
```

### Including figures
```latex
\includegraphics[width=\textwidth]{arXiv-2506.20555v1/filename.pdf}
```

### Physics notation
- Color representations: `$\bar{3}_c$`, `$6_c$`
- Wave function: `$\Psi_{\text{A}}^\pi(\boldsymbol{x})$`
- Binding energy: `$\Delta E$`
- RMS radius: `$r_{QQ}$`, `$r_{q\bar{q}}$`

## Audience Context

The presentation is for a hadron physics workshop. Audience may not be familiar with deep learning, so slides 4-8 provide ML background. Physics content should emphasize:
- Novel bound state predictions (pentaquarks)
- Comparison with established methods (GEM, DMC)
- Experimental signatures for discovery
