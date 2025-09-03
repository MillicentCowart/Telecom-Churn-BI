# Telecom-Churn-BI - Business Intelligence Project

## Project Overview
This project applies business intelligence methods to analyze telecom customer churn and uncover key drivers of attrition.  
Using a dataset of over 7,000 customers, the analysis identifies patterns in demographics, service usage, and billing that influence customer decisions to leave.  
The project delivers a cleaned dataset, exploratory analysis, interactive dashboard, and actionable recommendations for improving retention.  

---

## Objectives
- Identify the key drivers of customer churn  
- Create an interactive dashboard to monitor churn trends  
- Provide actionable recommendations to reduce churn   

---

## Files in this Repository

- `TelcoChurnSOW_8.25.25.docx` → Scope of Work  
- `TelcoChurn_data_raw_8.25.25.csv` → Raw data from Kaggle  
- `Telecom_Churn_DataClean.ipynb` → Python data cleaning and feature engineering
- `TelcoChurn_cleaned.plk` → Cleaned dataset with saved python datatypes
- `CleaningReportTelcoChurn8.26.25.pdf` → Data cleaning and feature engineering report
- `Telecom_Churn_EDA (1).ipynb` → Python exploratory data analysis and visualizations
- `TelcoReport_9.3.2025.html` → Project Report that includes Intro, Methodology, Analysis, Insights, Recommendations, and Conclusion

- `Dashboard_Demographic_ServiceAdoption.pdf` → Visualization1 of churn rate by demographics and service adoption
- `Dashboard_Demographic_ServiceAdoption.twb` → File to create visualization1
- `Dashboard_Payment_Contract.pdf` → Visualization2 of churn rate by payment method and contract type
- `Dashboard_Payment_Contract.twb` → File to create visualization2

---

## Dataset
**Source:** [Kaggle - Telco Customer Churn Dataset](https://www.kaggle.com/blastchar/telco-customer-churn)  
**Rows:** 7,043  
**Columns:** 21  

### Column Descriptions
- **customerID** → Unique identifier for each customer  
- **gender** → Male or Female  
- **SeniorCitizen** → Whether the customer is a senior citizen  
- **Partner** → Whether the customer has a partner  
- **Dependents** → Whether the customer has dependents  
- **tenure** → Number of months the customer has stayed with the company  
- **PhoneService** → Whether the customer has phone service  
- **MultipleLines** → Whether the customer has multiple lines 
- **InternetService** → Customer’s internet provider  
- **OnlineSecurity** → Whether the customer has online security add-on 
- **OnlineBackup** → Whether the customer has online backup add-on 
- **DeviceProtection** → Whether the customer has device protection add-on  
- **TechSupport** → Whether the customer has tech support add-on 
- **StreamingTV** → Whether the customer has streaming TV service 
- **StreamingMovies** → Whether the customer has streaming movies service 
- **Contract** → Type of contract  
- **PaperlessBilling** → Whether the customer uses paperless billing  
- **PaymentMethod** → Payment method  
- **MonthlyCharges** → The amount charged to the customer monthly  
- **TotalCharges** → The total amount charged to the customer over their tenure  
- **Churn** → Whether the customer left the company

### Feature Engineering
- **AvgMonthlyRevenue** → On average how much customers pay per month of tenure  
- **TenureGroup** → Tenure Groups: 0-1 years, 1-2 years, 2-4 years, or 4-6 years
- **NumServices** → How many optional services a customer has subscribed to  
- **IsAutoPay** → Autopay vs manual  
- **RiskScore** → Churn Risk Proxy. Combine short tenure + month-to-month contract + high monthly charges: High scores = High Churn Risk 
- **SeniorHighTech** → Senior Citizen with streaming and online sevice (high tech) 

---

## Tools & Technologies
- **Python:** pandas, matplotlib, seaborn for data cleaning and EDA    
- **Tableau:** for interactive dashboards  
- **Excel:** for data saving  

---

## Deliverables
- Cleaned dataset ready for analysis  
- Exploratory Data Analysis (EDA) report with visuals  
- Interactive Business Intelligence dashboard  
- Insights & Recommendations report

---

## Conclusions
- This project analyzed telecom customer data to identify the major drivers of churn and provide actionable strategies for retention. The analysis revealed four primary churn factors: customer demographics, contract type, adoption of value-added services, and billing/payment methods.  
- Key findings show that senior citizens without dependents or partners are at the highest risk of churn, especially when combined with month-to-month contracts and low adoption of support services. Additionally, reliance on electronic checks and lack of AutoPay enrollment strongly correlate with elevated churn rates.  
- These insights suggest that churn is not driven by a single factor but by an interplay of customer demographics, service engagement, and billing practices. Addressing these areas through targeted retention strategiesm such as promoting long-term contracts, incentivizing AutoPay, and increasing adoption of security and support services can significantly reduce churn.  
- Ultimately, by focusing on the needs of vulnerable customer segments and removing friction in service and payment experiences, the company can strengthen customer loyalty, improve profitability, and build a more resilient customer base.
