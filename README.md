# 💳 Credit Card Default Risk Prediction

---

## 📌 Project Overview

This project focuses on building a predictive model for credit card default risk using a dataset of 30,000 customer records. It includes end-to-end processes such as data understanding, cleaning, transformation, exploratory analysis, model training, and evaluation.

---

## 🧠 Features and Target

- **Target Variable**: `default_payment_next_month`  
  (1 = default, 0 = no default)

- **Key Features Used**:
  - Financial: `LIMIT_BAL`, `BILL_AMT1–6`, `PAY_AMT1–6`
  - Repayment History: `PAY_0` to `PAY_6`
  - Demographics: `AGE`, `SEX`, `EDUCATION`, `MARRIAGE`

---

## 🔍 Project Workflow

### 1. Data Understanding & Cleaning
- Missing values were identified and removed using `dropna()`.
- Standardization was applied to numerical features.
- Categorical features (like `SEX`, `EDUCATION`, `MARRIAGE`) were converted from numeric codes to text labels for better readability.

### 2. Exploratory Data Analysis
- Default class was imbalanced, with only ~22% of customers defaulting.
- Payment history features (`PAY_0`, `PAY_2`, `PAY_3`) showed the strongest correlation with defaults.
- Gender and marital status showed some disparity in default rates.

### 3. Model Development & Evaluation
- Logistic Regression was used to train the model.
- The model achieved **81% accuracy**.
- Precision for non-defaults was high, but recall for defaults was relatively low (24%), indicating many defaults were missed.
- Confusion matrix showed a high number of false negatives.

### 4. Ethical Considerations
- Features like `MARRIAGE` and `SEX` may introduce bias.
- Important to evaluate and mitigate any unfair penalization of demographic groups.

---

## 🛠 Technologies Used

- Python (Jupyter Notebook)
- Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

---

## 📌 Note

The complete **source code**, **cleaned dataset**, and **detailed project report** are available in a **private repository**.  
📩 **If you would like access for review or reference, feel free to contact me directly.**


