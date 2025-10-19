# Kaggle ML Explainability

This project is based on the **Kaggle "Machine Learning Explainability" course**.  
It demonstrates different techniques to interpret ML models using the FIFA 2018 dataset.

---

## 📂 Project Structure

```
├── data/
│ └── FIFA 2018 Statistics.csv
│
├── permutation_importance.ipynb
├── partial_plots.ipynb
├── SHAP_values.ipynb
└── Advanced_SHAP.ipynb
```

---

## 📘 Notebooks Overview

### 1. `permutation_importance.ipynb`
- Trains a **RandomForestClassifier** on the FIFA dataset.  
- Demonstrates **Permutation Importance** to identify which features most affect predictions.  
- Example insight: *Goals scored and attempts strongly drive predictions for "Man of the Match".*

### 2. `partial_plots.ipynb`
- Introduces **Partial Dependence Plots (PDPs)**.  
- Shows how varying one feature (e.g., possession, goals) affects model predictions while keeping others fixed.  
- Helps answer “what-if” questions.

### 3. `SHAP_values.ipynb` 
- Local explanations (single match): waterfall/force plots to see why the model predicted a certain probability.  

### 4. `Advanced_SHAP.ipynb`
- Extends SHAP analysis with:  
  - **Dependence plots** (feature effect + interactions).  
  - **Global beeswarm/bar plots** for many samples.  
  - Provides a more complete interpretability toolkit.

---

## ⚽ Dataset
**[FIFA 2018 Match Statistics](https://www.kaggle.com/datasets/mathan/fifa-2018-match-statistics)**  
Contains match-level features (e.g., goals, attempts, possession, fouls).  
Target: whether a player from the team won *"Man of the Match"* (`Yes`/`No`).

---

## 🛠️ Requirements
- Python 3.10+  
- pandas, numpy, scikit-learn  
- matplotlib, seaborn  
- shap  
- eli5  

