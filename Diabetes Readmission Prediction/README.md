# Diabetes Readmission Prediction

This project uses the UCI Diabetes 130-US hospitals dataset to build a machine learning model, that predicts whether a patient is likely to be readmitted within 30 days of hospital discharge.

## Objective

To predict 30-day hospital readmissions using patient demographics, admission information, and diagnosis codes. This helps healthcare providers identify high-risk patients early.

---

## Tools & Technologies

- Python (Pandas, Scikit-learn, Seaborn, Matplotlib)
- Machine Learning: Random Forest Classifier
- Dataset: [UCI ML Repository](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)
- Model Export: `pickle`
- Optional Deployment: Streamlit Web App

---

## Workflow

1. **Data Loading**: Used `ucimlrepo` to fetch dataset directly.
2. **Exploration**: Checked missing values, distributions, and data types.
3. **Preprocessing**:
   - Dropped sparse and irrelevant columns
   - Imputed missing values (`diag_1`, `race`, etc.)
   - Converted `readmitted` into binary classification target
   - One-hot encoded categorical features
4. **Modeling**:
   - Trained a Random Forest classifier
   - Achieved ~88% accuracy


