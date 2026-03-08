# Diabetes-Progression-Severity-Prediction-using-kNN
A beginner-friendly machine learning project that predicts **diabetes disease progression** using a **k-Nearest Neighbors (kNN) Regressor** on the classic scikit-learn Diabetes dataset.

---

## Overview 

This notebook walks through a complete ML regression workflow — from loading data to evaluating the effect of different values of `k` on model performance.

---

## Dataset

**Source:** [Diabetes Dataset — NCSU](https://www4.stat.ncsu.edu/~boos/var.select/diabetes.html) (built into `sklearn`)


---

## Topics Covered

1. **Dataset Loading** — using `sklearn.datasets.load_diabetes`
2. **Data Exploration** — feature inspection and scatter plot (bmi vs. target)
3. **Train-Test Split** — 50/50 split with fixed random seed for reproducibility
4. **kNN Regression** — fitting `KNeighborsRegressor` on training data
5. **Model Evaluation** — Mean Squared Error (MSE) on both train and test sets
6. **Effect of K** — comparing model performance across k = 1, 3, 5, 7, 30

---

## Key Results

| Model | Train MSE | Test MSE |
|-------|-----------|----------|
| kNN (default) | 2533.32 | 3719.89 |
| kNN (k=1) | 0.00 | ~higher |
| kNN (k=3) | lower | moderate |
| kNN (k=5) | moderate | moderate |
| kNN (k=30) | higher | lower |

> **Insight:** As `k` increases, the model becomes less overfit (lower test error) but may underfit at very large values of `k`.


---

## 👤 Author

**Diana Opiyo** — Part of a machine learning portfolio project.
