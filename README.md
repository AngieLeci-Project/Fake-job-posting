# Fake Job Posting Detection

Detecting fraudulent job postings using machine learning — Random Forest vs Logistic Regression.

---

## Overview

Online job scams are a growing problem for job seekers. This project builds a binary classifier to automatically detect fake job postings using a real-world dataset of 17,599 job records.

The project covers the full data science pipeline: from data cleaning and feature engineering to model training, evaluation, and comparison.

---

## Results

| Model | Accuracy | Precision | Recall | F1 Score |
|-------|----------|-----------|--------|----------|
| **Random Forest** | **97.8%** | **98%** | 56.7% | 71.9% |
| Logistic Regression | 95.3% | 80% | 4.7% | 8.8% |

> Random Forest outperformed Logistic Regression across all metrics and was selected as the final model.

---

## Tech Stack

| Category | Tools |
|----------|-------|
| Language | Python |
| Data Processing | pandas, NumPy |
| Machine Learning | scikit-learn |
| Visualization | matplotlib, seaborn |
| Environment | Jupyter Notebook |

---

## Dataset

- **Source:** [Kaggle — Real or Fake Job Posting Prediction](https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction)
- **Size:** 17,880 rows → 17,599 after duplicate removal
- **Features:** 18 columns including job title, description, company profile, requirements
- **Target:** `fraudulent` (0 = real, 1 = fake)

---

## Workflow

```
1. Data Loading & Exploration
        ↓
2. Data Cleaning
   - Removed 281 duplicate rows
   - Handled missing values
        ↓
3. Feature Engineering
   - Text preprocessing
   - Feature selection
        ↓
4. Model Training
   - Train-test split (80/20)
   - Random Forest Classifier
   - Logistic Regression
        ↓
5. Evaluation
   - Accuracy, Precision, Recall, F1-Score
   - Confusion Matrix
   - Model Comparison
```

---

## Key Findings

- Random Forest significantly outperformed Logistic Regression, especially in precision (98% vs 80%)
- Class imbalance was a key challenge — only ~4.8% of records are fraudulent
- The model achieves high precision, meaning very few real jobs are incorrectly flagged as fake
