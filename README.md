# Customer Churn Prediction and Data Analysis (SQL, Power BI & Random Forest)

## 📌 Project Overview
This project combines **Data Analysis, Predictive Modeling, and Business Intelligence Dashboards** to address the problem of **Customer Churn**.  
It involves:
- **SQL** for data preprocessing and churn-related queries  
- **Random Forest Model (ML)** for churn prediction  
- **Power BI Dashboards** (Before Prediction & After Prediction) with navigation between them  

The goal is to identify **why customers churn** and provide **predictive insights** to help businesses improve retention strategies.

---

## 🗂️ Dataset
- **Source**: CSV file (included in repository)  
- **Size**: ~6,400 rows and 30 columns  
- **Key Features (Columns)**:
  - `Customer_ID`, `Gender`, `Age`, `Married`, `State`
  - `Number_of_Referrals`, `Tenure_in_Months`, `Value_Deal`
  - `Phone_Service`, `Multiple_Lines`, `Internet_Service`, `Internet_Type`
  - `Online_Security`, `Online_Backup`, `Device_Protection_Plan`, `Premium_Support`
  - `Streaming_TV`, `Streaming_Movies`, `Streaming_Music`, `Unlimited_Data`
  - `Contract`, `Paperless_Billing`, `Payment_Method`
  - `Monthly_Charge`, `Total_Charges`, `Total_Refunds`, `Total_Extra_Data_Charges`, `Total_Long_Distance_Charges`, `Total_Revenue`
  - `Customer_Status`, `Churn_Category`, `Churn_Reason`  

- **Target Variable**:  
  - `Customer_Status` → Identifies whether the customer is **Churned / Retained / Joined**  
  - `Churn_Category` and `Churn_Reason` provide additional context for churned customers


---

## ⚙️ Tech Stack
- **SQL** – Data cleaning, feature extraction, and churn analysis  
- **Python (Scikit-learn)** – Random Forest for churn prediction  
- **Power BI** – Interactive dashboards with navigation buttons  

---

## 🧠 Machine Learning (Random Forest)
- Model: **Random Forest Classifier**  
- Input Features: Customer demographics, tenure, services, contract type, etc.  
- Output: **Predicted Churn (Yes/No)**  
- Evaluation: Accuracy, Precision, Recall, F1-score  
- Predicted results integrated back into **Power BI** for visualization  

---

## 📊 Dashboards
### 🔹 1. **Before Prediction (Summary Dashboard)**
- Overall churn rate & retention rate  
- Service-wise churn patterns  
- Contract type vs churn analysis  
- Revenue impact of churn  
- Filters for demographic & service segmentation  

### 🔹 2. **After Prediction (Prediction Dashboard)**
- Churn risk probability distribution  
- Predicted churned customers vs retained customers  
- Feature importance (from Random Forest)  
- Revenue loss forecast (based on predictions)  

### 🔹 🔄 Dashboard Navigation
- **Top-right navigation buttons** (`Summary ↔ Prediction`) allow switching between the two dashboards seamlessly.  
- **Prediction dashboard** is powered by the same dataset used for training the Random Forest model.  

<img width="1452" height="807" alt="Screenshot 2025-09-10 111215" src="https://github.com/user-attachments/assets/e91c95b6-49c9-45f3-8a94-b8c6f8106329" />
<img width="1456" height="805" alt="Screenshot 2025-09-10 111237" src="https://github.com/user-attachments/assets/66b21e3c-440f-4b7c-b32f-38be79f8c464" />


---

## 📈 Results & Insights
- Customers with **short tenure** and **month-to-month contracts** are most likely to churn.  
- **Fiber optic internet** customers churn more compared to DSL.  
- Customers without **security/backup add-ons** have higher churn probability.  
- ML model achieved **XX% accuracy** in predicting churn.  
- Power BI dashboards provide both **historical churn insights** and **predictive churn outcomes**.  

---

## 🚀 How to Run
1. Clone this repository  
   ```bash
   git clone https://github.com/PERAMPRAKASH/Customer-Churn-Prediction-SQL-PowerBI-RandomForest.git
