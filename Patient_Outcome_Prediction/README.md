# 🏥 Patient Outcome Prediction Using Real-Time Clinical Data

A healthcare machine learning project using a synthetic MIMIC-III-style dataset to predict patient outcomes (e.g., recovery) based on clinical and demographic data. This project demonstrates end-to-end implementation of data preprocessing, exploratory data analysis, feature engineering, and supervised classification modeling.

---

## 🎯 Objective

The objective of this project is to develop an accurate and interpretable classification model that predicts whether a patient will recover (`outcome = 1`) or not (`outcome = 0`) using real-time clinical features. This helps clinicians make timely, data-informed decisions.

---

## 🧾 Dataset Overview

**File**: `dental.csv`  
**Source**: Simulated data mimicking the structure of MIMIC-III  
**Features include**:
- Patient ID, age, gender
- Diagnosis, vital signs (heart rate, blood pressure, oxygen saturation)
- Lab results (white blood cell count)
- Treatment details
- Binary outcome (recovered = 1, not recovered = 0)

📄 Refer to the [Data Dictionary](./Data_Dictionary.pdf) for a detailed description of all features.

---

## 🧪 ML Workflow

![ML Workflow](./ML_Workflow_Diagram.pdf)

1. Load and inspect the dataset
2. Handle missing values
3. Encode categorical variables
4. Normalize features
5. Split into training and testing sets
6. Train classification models:
   - Logistic Regression
   - Random Forest
7. Evaluate performance:
   - Accuracy, ROC-AUC, F1-score, Confusion Matrix
8. Visualize key metrics and interpret results

---

## 📊 EDA Insights

- Outcome classes were balanced to some degree.
- Strong correlation between vitals (like heart rate, BP) and patient outcome.
- Certain diagnoses are more likely associated with poor outcomes.

---

## 📁 Project Structure

Patient_Outcome_Analysis/
├── dental.csv
├── Patient_Outcome_Prediction.ipynb
├── Data_Dictionary.pdf
├── ML_Workflow_Diagram.pdf
├── Summary_Report.pdf
└── README.md

yaml
Copy
Edit

---

## 📌 Recommendations

- Improve data quality by collecting more samples and features.
- Deploy model with monitoring in a clinical setting.
- Consider adding time-series vitals for higher temporal accuracy.
- Use explainability tools (e.g., SHAP) for clinician trust.
