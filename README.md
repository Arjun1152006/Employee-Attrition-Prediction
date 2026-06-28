# Employee Attrition Prediction using Machine Learning

Predict employee attrition using Machine Learning on the **IBM HR Analytics Employee Attrition Dataset**. This project demonstrates an end-to-end machine learning workflow, including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and HR-focused business recommendations.

---

## Project Overview

Employee attrition is a major challenge for organizations, leading to increased recruitment costs, training expenses, and productivity loss. This project builds a machine learning system that predicts whether an employee is likely to leave the company based on workplace and demographic factors such as job role, monthly income, overtime, work-life balance, and years at the company.

Three classification models were trained and compared to identify the most effective approach for predicting employee attrition.

**Best Model:** Logistic Regression

* **ROC-AUC:** 0.799
* **Recall:** 61.7%
* **Accuracy:** 74.8%

---

## Dataset

* **Dataset:** IBM HR Analytics Employee Attrition & Performance
* **Source:** Kaggle
* **Records:** 1,470 Employees
* **Features:** 35
* **Target Variable:** Attrition (Yes / No)

The dataset (`WA_Fn-UseC_-HR-Employee-Attrition.csv`) is included in this repository for educational purposes.

---

## Project Structure

```text
Employee-Attrition-Prediction/
│
├── analysis.ipynb
├── README.md
├── requirements.txt
├── summary.docx
├── WA_Fn-UseC_-HR-Employee-Attrition.csv
│
└── charts/
    ├── 01_attrition_by_department.png
    ├── 02_attrition_by_jobrole.png
    ├── 03_monthly_income_vs_attrition.png
    ├── 04_worklifebalance_vs_attrition.png
    ├── 05_years_at_company_vs_attrition.png
    ├── 06_confusion_matrices.png
    ├── 07_roc_curve.png
    └── 08_feature_importance.png
```

---

## Technologies Used

* Python 3.x
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

## Machine Learning Workflow

* Data Loading
* Data Cleaning & Preprocessing
* Exploratory Data Analysis (EDA)
* Feature Engineering
* One-Hot Encoding
* Feature Scaling
* Train-Test Split (80:20)
* Model Training

  * Logistic Regression
  * Random Forest
  * Gradient Boosting
* Model Evaluation
* Feature Importance Analysis
* HR Business Recommendations

---

## Exploratory Data Analysis

The notebook includes detailed visualizations to understand employee attrition patterns.

### Department-wise Attrition

* Attrition count by department
* Attrition rate by department

### Job Role Analysis

* Attrition rate by job role

### Salary Analysis

* Monthly income distribution
* Average monthly income comparison

### Work-Life Balance Analysis

* Attrition rate across work-life balance ratings

### Employee Tenure Analysis

* Years at company distribution
* Median years at company

### Model Evaluation

* Confusion matrices
* ROC Curve comparison
* Feature importance visualization

---

## Model Performance

| Model               |  Accuracy | Precision |    Recall | F1 Score |   ROC-AUC |
| ------------------- | --------: | --------: | --------: | -------: | --------: |
| Logistic Regression | **74.8%** |     34.1% | **61.7%** |    43.9% | **0.799** |
| Random Forest       |     84.4% |     57.1% |      8.5% |    14.8% |     0.772 |
| Gradient Boosting   |     84.0% |     50.0% |     23.4% |    31.9% |     0.792 |

**Selected Model:** Logistic Regression

Although Random Forest achieved higher accuracy, Logistic Regression was selected because it achieved the highest recall and ROC-AUC while remaining easily interpretable for HR decision-making.

---

## Top Predictive Features

The most influential factors contributing to employee attrition include:

1. Laboratory Technician Job Role
2. Overtime
3. Frequent Business Travel
4. Job Level
5. Total Working Years
6. Sales Representative Job Role
7. Business Travel Frequency
8. Education Field (Life Sciences)
9. Years Since Last Promotion
10. Sales Department

---

## Key Business Insights

* Sales department has the highest employee attrition rate (20.6%).
* Sales Representatives experience the highest attrition among all job roles (39.8%).
* Employees working overtime are significantly more likely to leave.
* Employees who resigned earned approximately **$2,000 less per month** than employees who stayed.
* Most attrition occurs during the first few years of employment.

---

## HR Recommendations

* Monitor employees with frequent overtime and provide workload support.
* Prioritize retention initiatives for Sales Representatives and Laboratory Technicians.
* Improve career progression opportunities for employees in high-risk job roles.
* Enhance work-life balance programs to improve employee satisfaction.
* Conduct regular retention discussions during employees' early years with the company.

---

## Future Improvements

* Hyperparameter tuning using GridSearchCV
* Apply SMOTE for handling class imbalance
* Explain predictions using SHAP values
* Deploy the model using Flask or FastAPI
* Build an interactive dashboard using Streamlit

---

## Installation

Clone the repository:

```bash
git clone https://github.com/<Arjun1152006>/Employee-Attrition-Prediction.git
```

Navigate to the project folder:

```bash
cd Employee-Attrition-Prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook analysis.ipynb
```

---

## Repository Topics

`machine-learning` `python` `employee-attrition` `classification` `scikit-learn` `data-science` `eda` `hr-analytics`

---

## Author

**Arjun P**

B.Tech – Artificial Intelligence & Machine Learning

Seshadri Rao Gudlavalleru Engineering College

---

## License

This project is developed for educational and internship purposes.
