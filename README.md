# PEDAS 2026 — Machine Learning Classification

A machine learning classification project developed for PEDAS 2026.

## Final Score

**Final score: `0.835325545`**

## Project Overview

This project predicts the category of each record using dataset features. The workflow includes data preprocessing, feature engineering, Random Forest model training, and prediction generation.

## Workflow

1. **Data loading** — Load the labeled training data and unlabeled prediction data.
2. **Data preprocessing** — Prepare the input data and normalize category labels.
3. **Feature engineering** — Extract features from domain information, URL characteristics, timestamps, and frequency-based information.
4. **Model training** — Train a Random Forest classifier on the labeled training data.
5. **Prediction** — Generate category predictions for the unlabeled records.

## Model Configuration

The final model uses `RandomForestClassifier` with the following parameters:

| Parameter | Value |
|---|---|
| `n_estimators` | `100` |
| `max_depth` | `None` |
| `min_samples_leaf` | `1` |
| `max_features` | `"sqrt"` |
| `class_weight` | `None` |
| `random_state` | `42` |
| `n_jobs` | `-1` |

## Repository Structure

```text
PEDAS-2026/
├── README.md
├── data/
│   ├── training.csv
│   └── predict.csv
├── notebooks/
│   └── pedas2026_final.ipynb
└── submission/
    └── submission_final.csv
```

## Dataset

- `training.csv` — Labeled data used to train the classifier.
- `predict.csv` — Unlabeled data used to generate predictions.

The notebook must be able to access these files at the paths configured in the code.

## How to Run

1. Clone or download this repository.
2. Open `notebooks/pedas2026_final.ipynb` in Google Colab or Jupyter Notebook.
3. Make sure the dataset files are accessible at the locations configured in the notebook.
4. Run the notebook cells in order to reproduce preprocessing, feature engineering, model training, and prediction.

## Output

The prediction workflow generates category predictions for the records in `predict.csv`. The final submission file is stored separately in the `submission/` directory.

## Disclaimer

This repository documents a machine learning project developed for PEDAS 2026. Check dataset ownership, redistribution permissions, and competition rules before publishing any competition data.
