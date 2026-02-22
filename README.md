#  Credit Risk Modelling System
![Python](https://img.shields.io/badge/Python-3.10+-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Classification-green)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![XGBoost](https://img.shields.io/badge/XGBoost-Boosting-red)
![Streamlit](https://img.shields.io/badge/Streamlit-Deployed-success)

An end-to-end **Machine Learning Classification Project** that predicts **Credit Risk** of loan applicants based on financial, demographic, and credit-related attributes.

🔗 **Live App:**  
**  

---

#  Project Overview

Financial institutions need to assess the creditworthiness of applicants to minimize loan defaults.

This project builds a complete ML pipeline to:

- Analyze applicant data  
- Identify risk-driving factors  
- Train multiple classification models  
- Compare performance  
- Deploy a credit risk prediction system  

---

##  Features

- Predict **Credit Risk (High / Low)** for loan applicants  
- Detailed **Exploratory Data Analysis (EDA)**  
- Feature selection using VIF to remove multicollinearity  
- Compare multiple classification algorithms  
- Analyze misclassified cases for better insights  
- Modular and scalable project structure  
- Deployment-ready architecture  

---

##  Problem Statement

Banks and lending institutions need to determine whether a loan applicant is **likely to default** or **repay successfully**.

This system predicts:

> **Credit Risk** (High / Low)

Using features such as:

- Applicant Age  
- Gender  
- Employment Type  
- Loan Amount  
- Sanctioned Amount  
- Credit History  
- Number of Dependants  
- Income Level  

This is a **Supervised Classification Problem**.

---

##  Dataset Description

The dataset contains structured loan applicant information.

###  Features

| Feature Name | Description |
|--------------|------------|
| age | Applicant's age |
| gender | Applicant's gender |
| employment_type | Type of employment |
| number_of_dependants | Number of dependants |
| income_level | Encoded income category |
| loan_amount | Loan amount requested |
| sanction_amount | Amount sanctioned by bank |
| principal_outstanding | Remaining principal amount |
| credit_history | Historical credit repayment status |
| processing_fee | Fee charged during loan processing |
| gst | GST applicable on loan |
| net_disbursement | Net loan disbursed |
| risk_flag | Target variable: High / Low risk |

###  Data Preprocessing

- Handling missing values  
- Encoding categorical variables  
- Feature scaling using StandardScaler  
- Removing multicollinear features using VIF  
- Outlier inspection  
- Reverse scaling for interpretability  

---

##  Exploratory Data Analysis (EDA)

EDA was performed using:

- Scatter plots  
- Distribution plots  
- Correlation heatmaps  
- Feature vs target visualization  

###  Key Insights

- Credit history strongly influences default risk  
- Loan amount and sanctioned amount are highly correlated  
- Certain income-employment combinations show higher default probability  
- Age has weak linear relationship but can interact with other features  

---

##  Models Implemented

The following classification models were trained and compared:

1. Logistic Regression  
2. Random Forest Classifier  
3. XGBoost Classifier  

---

##  Model Evaluation

Models were evaluated using:

- **Rank Ordering** – for stability of model ranking and decile performance  
- **KSS (Kolmogorov-Smirnov Statistic)** – to measure discrimination power between good and bad applicants  
- Optuna-optimized metrics for hyperparameter selection  

###  Model Comparison (Example Format)

| Model | KSS Score | Rank Ordering | Optuna Best Params |
|--------|-----------|---------------|------------------|
| Logistic Regression | — | — | — |
| Random Forest | — | — | — |
| XGBoost | — | — | — |

The best model was selected based on **highest KSS score and consistent rank ordering performance**.

---

## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone .https://github.com/AngadiAbhinay01/ML_Health_Premium_Predictiongit
   cd healthcare-premium-prediction
   ```
2. **Install dependencies:**:   
   ```commandline
    pip install -r requirements.txt
   ```
3. **Run jupyter notebook:**:   
   ```commandline
    jupyter notebook
   ```
4. **Run the Streamlit app:**:   
   ```commandline
    https://mlhealthpremiumprediction.streamlit.app/
   ```
---

##  Tech Stack

- **Python 3.10+** – Core programming language  
- **Pandas** – Data manipulation and preprocessing  
- **NumPy** – Numerical computations  
- **Matplotlib** – Data visualization  
- **Seaborn** – Statistical data visualization  
- **Scikit-learn** – Machine learning models and preprocessing  
- **XGBoost** – Gradient boosting regression model  
- **Jupyter Notebook** – Model development and experimentation  
- **Streamlit** – Interactive frontend deployment (optional)  

---

##  Key Learnings

- Importance of proper data preprocessing before model training  
- Feature scaling significantly impacts regression performance  
- Comparing multiple models improves reliability and robustness  
- Exploratory Data Analysis (EDA) helps uncover hidden data patterns  
- Reverse scaling improves real-world interpretability of predictions  
- Model evaluation metrics (RMSE, R²) must be interpreted together  

---

##  Future Enhancements

- Hyperparameter tuning using GridSearchCV or RandomSearchCV  
- Implement K-Fold Cross Validation for robust evaluation  
- Add SHAP for model explainability  
- Build REST API using FastAPI or Flask  
- Deploy on AWS / GCP / Azure  
- Add additional real-world health risk features  
- Implement automated model monitoring  

---

##  Author

**Abhinay Angadi**  

 Email: angadiabhinay2001@gmail.com  
 LinkedIn: https://linkedin.com/in/abhinay-angadi-541004159  
 GitHub: https://github.com/AngadiAbhinay01

---
---

## ⭐ If You Found This Project Helpful

If you found this project useful or insightful, please consider giving it a ⭐ on GitHub.  
Your support helps increase visibility and encourages further improvements!
