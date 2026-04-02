# 📞 Telco Customer Churn Prediction

Predicting which customers are likely to leave a telecommunications provider using Machine Learning.

## 📌 Project Overview
Customer churn happens when clients stop doing business with a company. In the telecom industry, retaining existing customers is often more cost-effective than acquiring new ones. This project uses the **IBM Telco Customer Churn dataset** to build a predictive model that identifies high-risk customers.

## 📊 Key Features of the Data
The dataset includes 7,043 customers and 21 features, categorized into:
* **Demographics:** Gender, Senior Citizen, Partner, Dependents.
* **Services:** Phone, Multiple Lines, Internet (DSL/Fiber optic), Online Security, Tech Support, Streaming TV/Movies.
* **Account Info:** Tenure, Contract Type, Payment Method, Monthly Charges, Total Charges.

## 🛠️ Technical Stack
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (Logistic Regression, Decision Trees)

## 🚀 Project Workflow

### 1. Data Cleaning & Preprocessing
* Dropped `customerID` as it provides no predictive value.
* Converted `TotalCharges` from string to numeric, handling empty strings as nulls.
* Applied **One-Hot Encoding** to categorical variables to prepare them for mathematical modeling.

### 2. Model Training & Evaluation
I implemented and compared two distinct models:
* **Logistic Regression:** Achieved ~79% accuracy. This model required feature scaling using `StandardScaler` to handle the variance between tenure and charges.
* **Decision Tree Classifier:** Achieved ~72% accuracy. This model provided excellent interpretability for feature importance.

## 📈 Insights & Results
The model revealed the following primary drivers of churn:
1.  **Contract Type:** Month-to-month contracts are the strongest indicator of churn.
2.  **Tenure:** Customers in their first 6 months are at the highest risk.
3.  **Internet Service:** Fiber optic users churn at a higher rate, likely due to higher price points.

## 💡 Business Recommendations
* **Encourage Long-term Contracts:** Offer small monthly discounts for switching from month-to-month to 1 or 2-year contracts.
* **Retention Programs:** Focus customer success efforts on new users within their first 90 days.
* **Service Bundling:** Promote "Tech Support" and "Online Security" add-ons, as customers with these services stay longer.

---
**Author:** siricodez
