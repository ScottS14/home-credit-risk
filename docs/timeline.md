# Credit-Risk Scoring
*Dataset ↠ Home-Credit Default Risk · 28 Jun → 24 Jul 2025*

| **Week** | **Dates (2025)** | **Focus & Objectives 🎯** | **Key Tasks 🛠** | **Done = 📦** |
|----------|-----------------|---------------------------|------------------|---------------|
| **1** | **28 Jun – 3 Jul** | **EDA + Baseline kick-off** | • Explore schema, missingness, class-imbalance heatmaps<br>• Draft `engineer_credit.py` (ratios, bureau aggregates)<br>• LightGBM 5-fold CV, W&B experiment | Notebook `eda_overview.ipynb`; `train.parquet`; LightGBM ROC & PR curves |
| **2** | 4 – 10 Jul | **Second baseline + Calibration** | • XGBoost 5-fold CV (reuse splits)<br>• 20-trial Optuna sweep on LightGBM params<br>• Calibration curve + Brier score; choose threshold for 95 % recall | MLflow/W&B runs; `baseline_cv.png`; calibration PNG |
| **3** | 11 – 17 Jul | **Interpretability & Docs** | • SHAP TreeExplainer: global beeswarm + 2 force plots<br>• Cost-impact table (false-neg vs false-pos) in README<br>• README v0.5 (Model Zoo, metric table) | SHAP figs in `/reports/figures/`; README updated |
| **4** | 18 – 24 Jul | **Package & Publish v1.0.0** | • Dockerfile (< 400 MB) via `uv`<br>• 3-min Loom demo (repro + insights)<br>• Tag v1.0.0; Zenodo DOI; LinkedIn draft | GHCR image; DOI badge; Loom link; release page |