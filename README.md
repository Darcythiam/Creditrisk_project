# German Credit Risk Classification

## Project Overview

This project builds a supervised machine learning classification model to predict whether a credit applicant is a **good** or **bad** credit risk using the German Credit dataset. The notebook follows a complete machine learning workflow, including data collection, exploratory data analysis, preprocessing, model training, cross-validation, hyperparameter tuning, and model interpretation.

This project demonstrates practical experience in:

- Supervised classification
- Data preprocessing for mixed feature types
- Exploratory Data Analysis (EDA)
- Model comparison and evaluation
- Hyperparameter tuning with GridSearchCV
- Feature importance analysis

---

## Objective

The goal of this project is to classify credit applicants into risk categories based on financial and demographic features. This can help support data-driven decision-making in lending and credit approval settings.

---

## Dataset

This project uses the **German Credit dataset** from OpenML.

### Dataset Characteristics

- **Instances:** 1,000
- **Features:** 20
- **Target Variable:** Credit risk (`good` or `bad`)

The dataset includes both:

- Numerical features
- Categorical features

Examples of variables include:

- Credit amount
- Loan duration
- Checking account status
- Age
- Credit history
- Employment status
- Housing status

---

## Technologies Used

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Scikit-learn

### Machine Learning Techniques

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Stratified Train/Test Split
- Stratified Cross-Validation
- GridSearchCV
- Feature Importance Analysis

---

## Project Workflow

## 1. Data Collection

The dataset was loaded from OpenML and separated into:

- Feature matrix `X`
- Target vector `y`

---

## 2. Exploratory Data Analysis

Initial exploration was performed to better understand the data and class structure.

### EDA included:

- Class distribution visualization
- Numerical feature histograms
- Correlation heatmap for numerical variables

### Key findings

- The dataset has a **class imbalance**, with more `good` credit cases than `bad`
- Numerical features vary widely in scale
- Some variables show moderate relationships, but no severe multicollinearity was observed among numerical features

---

## 3. Train/Test Split

The dataset was split into:

- **80% training data**
- **20% testing data**

A **stratified split** was used to preserve the class distribution in both sets.

---

## 4. Data Preprocessing

A preprocessing pipeline was created to handle numerical and categorical data separately.

### Numerical preprocessing

- Median imputation
- Standard scaling

### Categorical preprocessing

- Most frequent imputation
- One-hot encoding

This approach ensures that all features are properly prepared for machine learning models.

---

## 5. Model Selection and Training

Three classification models were trained and compared:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

To address class imbalance, models were configured using balanced class weights where appropriate.

---

## 6. Model Evaluation

Models were evaluated using several classification metrics:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

These metrics provide a more complete view of model performance, especially because the dataset is not perfectly balanced.

---

## 7. Cross-Validation

To obtain more reliable performance estimates, the project used **5-fold stratified cross-validation**.

Cross-validation helps:

- Reduce dependence on one train/test split
- Compare models more fairly
- Detect overfitting more effectively

---

## 8. Hyperparameter Tuning

The Random Forest model was further improved using **GridSearchCV**.

### Tuned parameters included:

- `n_estimators`
- `max_depth`
- `min_samples_split`
- `min_samples_leaf`
- `max_features`

The best model was selected based on **macro F1-score**.

---

## 9. Final Model Evaluation

After tuning, the best Random Forest model was evaluated on the test set using the same classification metrics.

The tuned model provided the strongest overall performance and a better balance between predictive accuracy and generalization.

---

## 10. Model Interpretation

Feature importance analysis was performed on the best Random Forest model to identify which variables most influenced predictions.

### Most influential features included:

- Checking account status
- Credit amount
- Loan duration
- Age
- Credit history

These features played the largest role in determining whether an applicant was predicted as a good or bad credit risk.

---

## Skills Demonstrated

### Data Science Skills

- Data cleaning
- Data preprocessing
- Exploratory Data Analysis
- Statistical interpretation
- Class imbalance awareness

### Machine Learning Skills

- Supervised classification
- Model comparison
- Cross-validation
- Hyperparameter tuning
- Performance evaluation
- Model interpretation

### Technical Skills

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Machine learning pipelines

### Installation

```bash
pip install pandas numpy matplotlib scikit-learn

```
Running the Project

Open the notebook with Jupyter:

```bash
jupyter notebook Project2_German_Credit2.ipynb
```
