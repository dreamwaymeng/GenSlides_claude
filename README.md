# DeepQuark Presentation Slides

Beamer presentation for "DeepQuark: Deep-Neural-Network Approach to Multiquark Bound States" (arXiv:2506.20555).

## Files

| File | Description |
|------|-------------|
| `slides.tex` | Main Beamer presentation (28 slides) |
| `slides.pdf` | Compiled PDF output |
| `arXiv-2506.20555v1/` | Source paper and figures |

## Slide Structure

1. **Title** (1 slide)
2. **Introduction** (2 slides): Multiquark zoo, computational challenges
3. **Deep Learning Background** (5 slides): ML basics, neural networks, NNQS, VMC
4. **DeepQuark Framework** (4 slides): Architecture, encoding, symmetry, innovations
5. **Results** (8 slides): Nucleon, Tcc, Tbb, T4c/T4b, pentaquarks, experimental search
6. **Conclusions** (3 slides): Summary, outlook, acknowledgments
7. **Backup** (5 slides): AL1 parameters, color bases, optimization, benchmarks

## Building

```bash
pdflatex slides.tex
pdflatex slides.tex  # Run twice for cross-references
```

## Requirements

- LaTeX with Beamer class
- Packages: tikz, amsmath, booktabs, graphicx
- Figures from `arXiv-2506.20555v1/`: `framework.pdf`, `Graph_multiquark.pdf`, `qqqFT.pdf`

## Key Results Presented

- **Tcc**: Molecular structure, -15 MeV binding, 55:45 color mixing
- **Tbb**: Compact diquark, -153 MeV binding, 0.33 fm core
- **T4c/T4b**: No bound states (resonances only)
- **Novel predictions**: P_ccbar(5715) at -3 MeV, P_bbbar(15569) at -14 MeV

## Authors

- Wei-Lin Wu (Peking University)
- Lu Meng (Ruhr-Universität Bochum / Southeast University)
- Shi-Lin Zhu (Peking University)
