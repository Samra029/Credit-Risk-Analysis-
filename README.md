

## 💳 Credit Risk Analysis – Flagging High-Risk Customers

### 📌 Objective  
This project focuses on building a machine learning model to evaluate the **creditworthiness** of customers using the "Give Me Some Credit" dataset. It aims to help financial institutions **reduce loan default rates** by identifying and flagging **high-risk individuals**.

---

### 🔍 Overview of Implementation

This notebook performs the following steps:

1. **Data Preprocessing**
   - Handled missing values using median imputation.
   - Applied **SMOTE** to balance the imbalanced dataset and address minority class underrepresentation.

2. **Feature Engineering**
   - Created and normalized features related to:
     - Monthly income
     - Debt ratio
     - Number of late payments (30–59, 60–89, 90+ days)
   - Removed outliers and scaled numerical features using **StandardScaler**.

3. **Model Training**
   - Trained and evaluated three models:
     - **Random Forest**
     - **Gradient Boosting**
     - **XGBoost**
   - Used train-test split (70–30) for evaluation.

4. **Model Evaluation**
   - Evaluated models using:
     - Accuracy
     - Classification report (Precision, Recall, F1-score)
     - Confusion matrix
     - ROC Curve and AUC score

---

###  Results & Outcome  
- **Random Forest Accuracy:** `86.39%`
- **Gradient Boosting Accuracy:** `86.41%`
- **XGBoost Accuracy:** `86.74%`

🔎 The **XGBoost classifier** slightly outperformed others, showing better generalization for identifying high-risk customers.

📊 The system provides a reliable method to flag potentially risky loan applicants and can be integrated into a credit evaluation pipeline to **reduce default rates** effectively.

---

### 🛠️ Tech Stack  
- Python (Pandas, NumPy, Scikit-learn, XGBoost)  
- Imbalanced-learn (SMOTE)  
- Seaborn & Matplotlib (for data visualization)

---

### 📁 Dataset  
- Dataset: [Give Me Some Credit - Kaggle](https://www.kaggle.com/c/GiveMeSomeCredit)

