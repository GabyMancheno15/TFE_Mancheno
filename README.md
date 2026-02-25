# TFE – QUILLAQUA: Predictive microclimate control (XGBoost + E_Ctrl supervisor)

This repository contains the notebook and data used in the TFE on predictive microclimate control in the QUILLAQUA experimental greenhouse. The approach combines multivariable forecasting (XGBoost) with a rule-based supervisor compatible with the existing reactive controller (E_Ctrl), preserving operational priorities, safety guards, hysteresis, and minimum on/off times.

## Files
- `Codigo_completo.ipynb`: end-to-end notebook (data extraction, preprocessing, model evaluation, and replay/shadow testing).
- `QDBR.sqlite`: SQLite database used in the analysis.

## How to run
1. Create a Python environment (recommended: Python 3.10+).
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
