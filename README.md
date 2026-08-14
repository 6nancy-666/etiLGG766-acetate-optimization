# etiLGG766

Dual-constrained genome-scale metabolic model of *Lacticaseibacillus rhamnosus* GG (LGG),
with the analysis code used in the accompanying manuscript.

## Contents

- `models/etiLGG766.xml` — dual-constrained (enzyme + thermodynamic) genome-scale
  metabolic model in SBML format
- `LGG_TOTAL_FINAL.ipynb` — Jupyter notebook with the complete analysis pipeline:
  model curation, MEMOTE quality assessment, flux balance analysis, Bayesian medium
  optimization, counterfactual / flux-envelope / knockout analyses, and prediction-error
  evaluation

## Requirements

- Python 3.9+
- COBRApy ≥ 0.26.0, scikit-optimize, pandas, numpy
- GLPK linear solver
- MATLAB + GECKO 3.0 (only for the enzyme-constraint construction block)

## Quick start

```bash
pip install cobra scikit-optimize pandas numpy
jupyter notebook LGG_TOTAL_FINAL.ipynb
