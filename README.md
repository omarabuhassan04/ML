# Machine Learning — Cardiovascular Disease Prediction

A Machine Learning project for cardiovascular disease prediction using the CARDIO dataset. Four classification models are trained and compared — Logistic Regression, Random Forest, Gradient Boosting, and Support Vector Machine (SVM) — each tested across multiple hyperparameter configurations. Models are evaluated using Accuracy, F1 Score, AUC-ROC, and Confusion Matrix on train, validation, and test splits.

## Dataset

- **Source:** `cardio_train.csv` (semicolon-separated)
- **Target:** `cardio` — 1 (has cardiovascular disease) / 0 (no disease)
- **Features:** Age, gender, height, weight, blood pressure, cholesterol, glucose, smoking, alcohol, activity

## Methodology

1. **Preprocessing** — Dropped ID column, converted age from days to years, label encoding, standard scaling
2. **Data Split** — Train (70%) / Validation (15%) / Test (15%) with stratification
3. **Model Training** — Each model trained with 5 different hyperparameter configurations
4. **Evaluation** — Accuracy, F1 Score, AUC-ROC, Confusion Matrix, ROC Curve plots

## Models & Hyperparameters

| Model | Key Hyperparameters Tested |
|-------|---------------------------|
| Logistic Regression | solver (lbfgs, liblinear, saga), C (0.5–2.0) |
| Random Forest | n_estimators (100–500), max_depth (None–20) |
| Gradient Boosting | n_estimators (100–500), learning_rate (0.01–0.1), max_depth (3–5) |
| SVM | kernel (rbf, linear, poly), C (0.5–2.0) |

## Evaluation Metrics

- **Accuracy** — Overall correct predictions
- **F1 Score** — Balance between precision and recall
- **AUC-ROC** — Model's ability to distinguish between classes
- **Confusion Matrix** — Breakdown of true/false positives and negatives

## Tools & Libraries

`Python` · `Pandas` · `Scikit-learn` · `Matplotlib` · `StandardScaler` · `LabelEncoder` · `Tabulate`

## Repository Structure

```
ML/
├── final_ml.ipynb    # Main Jupyter Notebook
├── ML report.docx    # Project report
└── README.md
```

## Author

**Omar Abuhassan**
