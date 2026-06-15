Fake Job Posting Detection

Detecting fraudulent job postings using machine learning — Random Forest vs Logistic Regression.

Overview

Online job scams are a growing problem for job seekers. This project builds a binary classifier to automatically detect fake job postings using a real-world dataset of 17,599 job records.
The project covers the full data science pipeline: from data cleaning and feature engineering to model training, evaluation, and comparison

Results

Random Forest: Accuracy 97.8%, Precision 98%, Recall 56.7%, F1 Score 71.9%
Logistic Regression: Accuracy 95.3%, Precision 80%, Recall 4.7%, F1 score 8.8%
Random Forest outperformed Logistic Regression across all metrics and was selected as the final model.


Source: Kaggle — Real or Fake Job Posting Prediction (https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction)
Size: 17,880 rows → 17,599 after duplicate removal
Features: 18 columns including job title, description, company profile, requirements
Target: fraudulent (0 = real, 1 = fake)
