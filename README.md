# German Credit Risk Classification

## Project Overview

This project builds a supervised machine learning pipeline to classify whether a credit applicant is a **good** or **bad** credit risk using the German Credit dataset.

The work is structured in two stages:

- **Core Model Development** – data preprocessing, model training, and baseline evaluation  
- **Model Refinement & Analysis** – hyperparameter tuning, deeper evaluation, and model interpretation  

Together, these stages demonstrate a complete and iterative machine learning workflow.

---

## Notebooks

| Notebook | Purpose |
|---|---|
| `Project2_German_Credit2.ipynb` | Baseline model: data preprocessing, EDA, and initial model training |
| `05_credit_risk_model_tuning_and_analysis.ipynb` | Extended work: hyperparameter tuning, cross-validation, and model improvement |

---

## Objective

Classify credit applicants into risk categories based on financial and demographic features to support data-driven decision-making in lending.

---

## Dataset

- **Source:** OpenML (German Credit dataset)  
- **Instances:** 1,000  
- **Features:** 20  
- **Target:** `good` vs `bad` credit risk  

Includes both numerical and categorical variables such as credit amount, loan duration, employment status, and credit history.

---

## Workflow

### 1. Data Exploration
- Class distribution analysis  
- Feature visualization  
- Correlation analysis  

### 2. Preprocessing
- Numerical: imputation + scaling  
- Categorical: imputation + one-hot encoding  
- Combined using a preprocessing pipeline  

### 3. Baseline Modeling
- Logistic Regression  
- Decision Tree  
- Random Forest  

### 4. Evaluation
- Accuracy, Precision, Recall, F1-score  
- ROC-AUC  
- Confusion matrix  

### 5. Cross-Validation
- Stratified 5-fold cross-validation  
- Improved reliability of performance estimates  

### 6. Model Improvement (Project 4)
- Hyperparameter tuning using GridSearchCV  
- Optimization of Random Forest parameters  
- Focus on macro F1-score  

### 7. Final Model & Interpretation
- Best model evaluated on test data  
- Feature importance analysis  
- Identification of key predictors (credit amount, duration, account status, etc.)

---

## Technologies

- Python  
- Pandas, NumPy  
- Matplotlib  
- Scikit-learn  

---

## Key Takeaways

- Proper preprocessing is critical for mixed-type datasets  
- Cross-validation improves model reliability  
- Hyperparameter tuning significantly improves performance  
- Feature importance helps interpret model decisions  

---

## Skills Demonstrated

- Data preprocessing and feature engineering  
- Model selection and comparison  
- Cross-validation and hyperparameter tuning  
- Model evaluation and interpretation  

---

## Running the Project

```bash
pip install pandas numpy matplotlib scikit-learn
jupyter notebook Project2_German_Credit2.ipynb
