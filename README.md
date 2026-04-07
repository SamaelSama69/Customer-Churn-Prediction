# 📊 Customer Churn Prediction – AlphaCom

🚀 **End-to-End Machine Learning Project | Business-Focused Data Analytics**

---

## 📌 Project Overview

Customer churn is one of the most critical challenges in the telecom industry, with **industry churn rates ranging between 20–30%**. This project builds a **data-driven churn prediction system** to help businesses proactively identify customers at risk of leaving and optimize retention strategies.

This project simulates a real-world telecom company (**AlphaCom**) and focuses on **transforming raw customer data into actionable business insights** using machine learning.

---

## 🎯 Business Problem

- Increasing churn is directly impacting:
  - 💰 Revenue
  - 📉 Customer Lifetime Value (CLV)
  - 📊 Profitability

- Traditional retention strategies are:
  - Reactive
  - Costly (blanket discounts)
  - Inefficient

👉 **Goal:** Build a predictive model to identify high-risk customers and enable **targeted retention strategies**.

---

## 📂 Dataset Overview

- 📊 **12,055 customer records**
- 📈 **20 features**
- 🎯 Target Variable: `Churn` (Yes/No)

### Key Feature Groups:
- **Demographics**: Gender, SeniorCitizen, Partner
- **Services**: InternetService, OnlineSecurity, TechSupport
- **Account Info**: Contract, PaymentMethod, Billing
- **Usage/Cost**: Tenure, MonthlyCharges, TotalCharges

---

## 🔍 Key Insights from EDA

- ⚠️ **27.9% churn rate** → realistic class imbalance  
- 📉 **Low tenure customers churn more frequently**
- 💸 **Higher monthly charges → higher churn probability**
- 📄 **Month-to-month contracts have highest churn**
- 🛠️ Lack of **Tech Support & Security services increases churn risk**

👉 **Conclusion:** Churn is driven by a combination of **pricing, contract flexibility, and service experience**.

---

## 🧹 Data Preprocessing Highlights

✔ Removed **24 duplicate records**  
✔ Handled missing & invalid values using **business logic (not naive imputation)**  
✔ Converted inconsistent data types  
✔ Standardized categorical variables  
✔ Prevented **data leakage** (excluded `TotalCharges` from modeling)  
✔ Applied **stratified 70/30 train-test split**

💡 Result: Clean, stable dataset → improved model reliability and generalization

---

## ⚙️ Modeling Approach

### 🧪 Baseline Model
- Logistic Regression
- Focus on **interpretability + business insights**

### 🚀 Advanced Models Tested
- Random Forest
- Gradient Boosting
- XGBoost

### 🎯 Evaluation Metrics
- AUC-PR (Primary metric)
- Recall (churn detection priority)
- F1-score

---

## 🏆 Final Model Selection

✅ **Gradient Boosting (Untuned)** chosen because:

- Strong balance of:
  - Accuracy
  - Interpretability
  - Stability
- Better **business alignment** vs overly complex models

---

## 📈 Business Impact

This model enables:

- 🎯 **Targeted retention campaigns**
- 💰 Reduced cost vs blanket discounts
- 🔍 Early identification of high-risk customers
- 📊 Better allocation of retention budget

### 📊 Strategic Benefits:
- Improve **Customer Lifetime Value (CLV)**
- Reduce churn-driven revenue loss
- Enable **data-driven decision making**

---

## 🧠 Key Takeaways

- Churn is **multi-factorial**, not driven by a single variable
- Early lifecycle (low tenure) is **critical intervention window**
- Service quality (support, security) plays a **major role**
- Data quality directly impacts **model performance & trust**

---

## 🛠️ Tech Stack

- **Python**
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 📁 Project Structure

```
├── notebook/
│   └── Customer_Churn_Notebook.ipynb
├── report/
│   └── Final_Report.pdf
├── data/
│   └── churn_dataset.csv
├── README.md
```

---

## 🚀 Future Improvements

- Hyperparameter tuning for boosted models
- Deployment using Flask / FastAPI
- Real-time, low latency churn prediction pipeline
- Integration with CRM systems

---

## 👨‍💻 Author

**Sham Solanki**  
Data Analyst | Machine Learning Enthusiast  

---

## ⭐ Why This Project Stands Out

✔ Strong **business + technical integration**  
✔ Focus on **real-world constraints (data leakage, imbalance)**  
✔ Emphasis on **interpretability (not just accuracy)**  
✔ Clear **actionable insights for stakeholders**
