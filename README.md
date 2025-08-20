# 🏦 Loan Approval Prediction — End-to-End  

This notebook is a complete starter for **Loan Approval Prediction** on a Kaggle-style dataset.  
It demonstrates how to build, evaluate, and compare machine learning models in an end-to-end workflow.  

---

## 📌 Project Overview  
The goal is to predict whether a loan application will be **Approved (Y)** or **Rejected (N)** based on applicant details such as income, credit history, and property area.  

This project covers:  
- ✅ Data loading & quick checks  
- ✅ Preprocessing (missing values, categorical encoding, train/test split)  
- ✅ Handling imbalanced data (class weights, SMOTE)  
- ✅ Models: **Logistic Regression** vs **Decision Tree**  
- ✅ Metrics: Precision, Recall, F1-score, ROC-AUC, Confusion Matrix  
- ✅ Threshold tuning for Logistic Regression using **Precision-Recall Curve**  

---

## 📂 Project Structure  
├── Loan_Approval_Prediction.ipynb # Main training & evaluation notebook
├── sample_loan_approval.csv # Sample dataset
├── README.md # Project documentation



---

## 📊 Dataset  
Each record contains the following fields:  

- **Loan_ID** – Unique Loan Identifier  
- **Gender** – Male / Female  
- **Married** – Yes / No  
- **Dependents** – Number of dependents  
- **Education** – Graduate / Not Graduate  
- **Self_Employed** – Yes / No  
- **ApplicantIncome** – Income of applicant  
- **CoapplicantIncome** – Income of co-applicant  
- **LoanAmount** – Loan amount (in thousands)  
- **Loan_Amount_Term** – Loan repayment term (in days)  
- **Credit_History** – Credit history meets guidelines (1/0)  
- **Property_Area** – Urban / Semiurban / Rural  
- **Loan_Status** – Target variable (Y = Approved, N = Rejected)  

---

## ⚙️ Workflow  

### 1. Data Preprocessing  
- Handle missing values  
- Encode categorical variables  
- Scale numerical features  
- Train/Test split  

### 2. Handling Imbalanced Data  
- **Option 1:** `class_weight="balanced"` for Logistic Regression  
- **Option 2:** **SMOTE** oversampling for minority class  

### 3. Model Training  
- **Logistic Regression** (baseline & threshold tuning)  
- **Decision Tree** (rule-based learning)  

### 4. Model Evaluation  
We use multiple metrics for fair comparison:  
- Confusion Matrix  
- Precision, Recall, F1-score  
- ROC-AUC score  
- Precision-Recall Curve for threshold tuning  

---

## 📈 Results  

### Confusion Matrix Example  
|                | Predicted Approved (Y) | Predicted Rejected (N) |
|----------------|-------------------------|-------------------------|
| **Actual Approved (Y)** | True Positive (TP) | False Negative (FN) |
| **Actual Rejected (N)** | False Positive (FP) | True Negative (TN) |

- **Logistic Regression**: Better at generalization, stable with threshold tuning.  
- **Decision Tree**: Captures complex rules but may overfit.  

---
