# TFE – QUILLAQUA: Predictive microclimate control with XGBoost + E_Ctrl supervisor

This repository contains the source code and analysis artifacts developed for a Master’s Final Project (TFE) focused on predictive microclimate control in an experimental greenhouse within the QUILLAQUA architecture. The approach combines a multivariable forecasting module (XGBoost) with a rule-based supervisor compatible with the existing reactive controller (E_Ctrl), preserving operational priorities, safety guards, hysteresis, and minimum on/off times.

## Repository contents
- `notebooks/`  
  Jupyter notebooks used for data extraction, preprocessing, feature engineering, model training/evaluation, and replay/shadow testing.
- `src/`  
  Auxiliary Python modules (utilities for metrics, psychrometric calculations, supervisor logic, plotting, and I/O).
- `data/`  
  Input data used in the analysis.
  - If confidentiality applies, this folder contains only anonymized subsets and/or aggregated exports required to reproduce the reported figures and tables.
- `results/`  
  Generated artifacts (tables, metrics, and summary outputs) used to build the thesis results section.
- `docs/`  
  Documentation and supporting material (figures, schemas, and notes).

## Data availability
- If a local SQL database is provided, it is expected under:
  - `data/QUILLAQUA.sqlite` (or equivalent filename)
- If the full database cannot be shared due to confidentiality constraints, the repository includes:
  - derived/aggregated datasets and the scripts required to reproduce the analysis pipeline on the original database.

**No credentials are stored in this repository.**

## Reproducibility and execution
1. Create a Python environment (recommended: Python 3.10+).
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
