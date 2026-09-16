# Diabetes Risk Factor Analysis

## Overview
This project analyzes the Pima Indians Diabetes dataset to identify which 
clinical factors most strongly predict diabetes, using exploratory data 
analysis, statistical distribution checks, and a predictive model. The 
analysis combines a data analytics approach with clinical context from my 
background as a registered nurse.

## Problem Statement
As a clinical nurse, I've seen how late diabetes diagnosis affects patient 
outcomes. This project answers: **Which clinical factors most strongly 
predict diabetes, and how can healthcare providers use this to prioritize 
screening?**

## Dataset
768 female patients, 8 clinical features (Glucose, BMI, Blood Pressure, 
Insulin, Age, Pregnancies, Skin Thickness, Diabetes Pedigree Function).  
Source: [Pima Indians Diabetes Database (Kaggle)](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)

## Key Findings
- **Glucose is the strongest single predictor of diabetes** (correlation = 
  0.50), with diabetic patients averaging 142 mg/dL vs 111 mg/dL in 
  non-diabetic patients.
- **Insulin and BMI are secondary but meaningful indicators** — diabetic 
  patients show markedly higher insulin (188 vs 117) and moderately higher 
  BMI (35.4 vs 30.8).
- **Age is a moderate risk factor** — diabetic patients are on average 6 
  years older.
- **Blood Pressure is the weakest standalone predictor** in this dataset.
- **Insulin is highly skewed** (skewness = 3.02, kurtosis = 13.76), with 
  51 patients (6.6%) identified as statistical outliers.
- A **logistic regression model** achieved 77% accuracy, but only 65% 
  recall on diabetic cases — meaning roughly 1 in 3 diabetic patients were 
  missed, which matters more than accuracy alone in a screening context.

## Recommendations
- Prioritize glucose and BMI screening as the strongest indicators, 
  especially in older patients.
- Treat the model as a screening aid, not a diagnostic tool — flagged 
  patients still require clinical follow-up.
- Future work: address class imbalance and Insulin's outliers to improve 
  recall for diabetic cases specifically.

## Tools Used
Python (pandas, numpy, matplotlib, seaborn, scikit-learn) in Jupyter Notebook

## Methodology
1. Data quality check (missing values, implausible zeros)
2. Distribution check (skewness, kurtosis, IQR outlier detection)
3. Class balance check
4. Exploratory analysis — group comparisons and boxplots (Glucose, BMI, Age)
5. Correlation heatmap
6. Logistic regression model with feature importance

## View the Full Analysis
📓 [Diabetes_Risk_Analysis.ipynb](./Diabetes_Risk_Analysis.ipynb)

## About Me
Odoh Ekenedirichukwu J. — Registered Nurse with 3+ years of clinical 
experience in Ophthalmic Nursing, transitioning into Data Analytics. 
Currently studying Excel, Power BI, Python, and SQL.  
[LinkedIn](https://linkedin.com/in/kene08)
