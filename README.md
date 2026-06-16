# Breast Cancer Classification Using Machine Learning Models

## Overview

This project presents a comparative analysis of multiple machine learning algorithms for binary classification of breast cancer data. The goal is to evaluate different classical and ensemble learning methods and identify the most effective model based on predictive performance.

The dataset used is the **Breast Cancer Wisconsin dataset** from Scikit-learn.

---

## Dataset Description

* Source: Scikit-learn Breast Cancer Dataset
* Samples: 569 patients
* Features: 30 numerical features
* Target:

  * `0` → Malignant
  * `1` → Benign

---

## Objective

The main objectives of this project are:

* Compare multiple machine learning models on a medical dataset
* Evaluate performance using F1-score and classification metrics
* Identify the most robust model for medical diagnosis tasks

---

## Machine Learning Models

The following models were implemented:

### 1. Support Vector Machine (SVM)

* Uses margin-based classification
* Requires feature scaling

### 2. Gaussian Naive Bayes

* Probabilistic classifier
* Assumes feature independence

### 3. Random Forest

* Ensemble of decision trees
* Robust to noise and overfitting

### 4. Gradient Boosting Models

* XGBoost
* LightGBM
* CatBoost

These models are widely used for structured medical datasets.

---

## Data Preprocessing

* Train-test split (80/20)
* Feature scaling using StandardScaler (for SVM and Naive Bayes)
* No missing values in dataset

---

## Evaluation Metrics

Model performance was evaluated using:

* Accuracy
* Precision
* Recall
* F1-score (primary metric)
* Confusion Matrix

F1-score was selected as the main metric due to its importance in medical diagnosis tasks.

---

## Results

| Model         | F1-score |
| ------------- | -------- |
| SVM           | 0.986    |
| CatBoost      | 0.979    |
| Naive Bayes   | 0.972    |
| Random Forest | 0.972    |
| LightGBM      | 0.972    |
| XGBoost       | 0.965    |

---

## Best Model

The **Support Vector Machine (SVM)** achieved the highest performance with an F1-score of **0.9861**.

---

## Key Insights

* SVM performs best for this dataset due to strong decision boundaries in low-dimensional feature space
* Ensemble methods (CatBoost, Random Forest) also perform competitively
* Boosting models provide stable performance but require tuning for further improvement
* Feature scaling significantly impacts model performance

---

## Technologies Used

* Python
* Pandas, NumPy
* Scikit-learn
* XGBoost, LightGBM, CatBoost
* Matplotlib, Seaborn

---

## Conclusion

This study demonstrates that classical machine learning models, particularly SVM, can achieve excellent performance on structured medical datasets. Ensemble methods also provide strong alternative solutions for classification tasks in healthcare applications.

---
