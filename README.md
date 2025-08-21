# Heart Disease Prediction (Logistic Regression)

[![Made with Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![scikit-learn](https://img.shields.io/badge/ML-scikit--learn-yellow.svg)](https://scikit-learn.org/)

A clean, reproducible machine‑learning mini‑project that predicts the presence of **heart disease** from demographic, clinical, and lifestyle features.  
This repo is designed as a **portfolio showcase**: it includes EDA plots, feature preprocessing, a **Logistic Regression** model, and an exportable **classification report**.

## Key Features
- Exploratory Data Analysis: histograms, countplots, and a correlation heatmap.
- Data prep: one‑hot encoding for categoricals and `StandardScaler` for numeric features.
- Model: `LogisticRegression` with train/test split and metrics.
- Artifacts: saved figures in `figures/` and a `model_classification_report.csv` after running the notebook.

## Dataset
- **Not included** in the repository. Place your CSV at: `data/heart_disease_dataset.csv`.
- Make sure your columns match the notebook (e.g., common fields like `Age`, `Cholesterol`, plus categoricals such as `Gender`, `Smoking`, `Alcohol Intake`, `Family History`, `Diabetes`, `Obesity`, `Exercise Induced Angina`, `Chest Pain Type`).  
- If you use a public dataset, credit the source here.

## How to Run (Conda)
```bash
# 1) Create and activate the environment
conda env create -f environment.yml
conda activate hd-pred

# 2) (Optional) Jupyter Lab
# conda install -c conda-forge jupyterlab

# 3) Put your data file here
#   data/heart_disease_dataset.csv

# 4) Launch Jupyter and run the notebook top-to-bottom
jupyter notebook notebooks/heart_disease_prediction.ipynb
```

Alternatively with pip:
```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
# source .venv/bin/activate

pip install -r requirements.txt
jupyter notebook notebooks/heart_disease_prediction.ipynb
```

## Repository Structure
```
heart-disease-prediction-portfolio/
├─ notebooks/
│  └─ heart_disease_prediction.ipynb
├─ data/                         # place heart_disease_dataset.csv here (not committed)
├─ figures/                      # auto-saved charts when you run the notebook
├─ artifacts/                    # outputs like model_classification_report.csv
├─ assets/                       # add screenshots or a cover image for README/LinkedIn
├─ requirements.txt
├─ environment.yml
├─ .gitignore
├─ LICENSE
└─ README.md
```

## Results
- After running, you'll get a **classification report** (precision, recall, F1) saved as `model_classification_report.csv`.
- Example EDA visuals are saved into the `figures/` directory.

## Reuse
- MIT licensed. Fork and adapt freely.
- Suggestions welcome via issues or pull requests.
