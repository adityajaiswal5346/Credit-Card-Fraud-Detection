# Credit-Card-Fraud-Detection

## 📌 Overview  
This project applies **Machine Learning** to detect fraudulent transactions in credit card data.  
The dataset is highly **imbalanced** (fraudulent cases are very rare), so the project explores techniques like **resampling, class weighting, and advanced models** to handle it.  

Fraud detection is critical in finance to prevent monetary loss and protect customers.  

---

## 🗂 Dataset  
- Dataset used: [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)  
- Contains **284,807 transactions** made by European cardholders in 2 days.  
- Features:  
  - `Time` → Seconds elapsed since the first transaction.  
  - `Amount` → Transaction amount.  
  - `V1` … `V28` → PCA-transformed features (anonymized).  
  - `Class` → Target variable (`0 = Legit`, `1 = Fraud`).  

⚠️ Dataset is **highly imbalanced** (~0.17% frauds).  

---

## ⚙️ Tech Stack  
- **Language:** Python  
- **Libraries:**  
  - `pandas`, `numpy` → Data handling  
  - `matplotlib`, `seaborn` → Visualization  
  - `scikit-learn` → ML models (Logistic Regression, Random Forest)  
  - `imbalanced-learn` → Handle class imbalance (SMOTE, undersampling)  
  - `lightgbm` → Gradient boosting model  
  - `shap` → Model interpretability  

---

## 📊 Approach  
1. **Data Preprocessing**  
   - Normalized `Amount` feature (log transform).  
   - Dropped `Time`
