# 🏠 Mortgage_Default_Predict

## 📘 Project Overview
This project focuses on predicting **mortgage default risk** using borrower-level data from **Freddie Mac Single-Family Loan-Level Dataset**.  
The goal is to develop a data-driven model that identifies early warning signals of default and helps assess loan portfolio risk exposure.

---

## 📂 Data

### 🔹 Data Source
- **Freddie Mac Single-Family Loan-Level Dataset**
  - https://drive.google.com/drive/folders/1X76auekeBb2DXpF8Q45CkwFJO8JnyQd0?usp=share_link
- Data includes loan-level attributes such as:
  - Borrower credit quality (e.g., Credit Score, DTI)
  - Loan structure (e.g., LTV, CLTV, interest rate)
  - Property characteristics (e.g., occupancy status, property state)
  - Performance variables (e.g., delinquency status)

---

### 🔹 Key Variables Used
| Category | Variables |
|-----------|------------|
| **Borrower Attributes** | `Credit Score`, `DTI`, `Number of Borrowers` |
| **Loan Structure** | `Original LTV`, `CLTV`, `Interest Rate`, `Original Loan Term`, `UPB` |
| **Performance** | `Current Loan Delinquency Status`, `Loan Age`, `Remaining Months` |
| **Property Info** | `Property State`, `Occupancy Status` |
| **Target Variable** | `Default` (1 = defaulted, 0 = active or paid off) |

---

## 🔍 Data Preprocessing (EDA → Modeling Preparation)

1. **Data Cleaning**
   - Removed duplicate records and invalid entries  
   - Handled missing values using median/mode imputation  
   - Removed non-informative columns (e.g., Loan Sequence Number, First Payment Date)

2. **EDA (Exploratory Data Analysis)**
   - Univariate and bivariate analysis to explore relationships with `Default`  
   - Examined distributions, outliers, and correlation heatmaps  
   - Identified imbalanced class issue (`Default`: ~0.4%)
   
