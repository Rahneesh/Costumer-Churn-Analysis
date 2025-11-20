Costumer churn analysis using IBM Telco data

1. Data used: https://www.kaggle.com/datasets/yeanzc/telco-customer-churn-ibm-dataset
Insights:
    The dataset includes customer details and service usage information from a telecommunications provider. The key features are:
    customerID – A unique ID assigned to each customer.
    gender – The customer’s gender (Male/Female).
    SeniorCitizen – Identifies if the customer is a senior citizen (1 = Yes, 0 = No).
    Partner – Shows whether the customer has a partner (Yes/No).
    Dependents – Indicates if the customer has dependents (Yes/No).
    tenure – The number of months the customer has been with the company.
    PhoneService – Specifies if the customer has phone service (Yes/No).
    MultipleLines – Indicates whether multiple phone lines are subscribed (Yes/No/No phone service).
    InternetService – Type of internet connection used (DSL, Fiber optic, No).
    OnlineSecurity – Whether the customer has online security (Yes/No/No internet service).
    OnlineBackup – Shows if the customer uses online backup services (Yes/No/No internet service).
    DeviceProtection – Indicates if device protection is activated (Yes/No/No internet service).
    TechSupport – Shows whether the customer has tech support service (Yes/No/No internet service).
    StreamingTV – Indicates if TV streaming is used (Yes/No/No internet service).
    StreamingMovies – Indicates if movie streaming is used (Yes/No/No internet service).
    Contract – Contract type (Month-to-month, One year, Two year).
    PaperlessBilling – Whether billing is paperless (Yes/No).
    PaymentMethod – Customer’s payment method (Electronic check, Mailed check, Bank transfer, Credit card).
    MonthlyCharges – Monthly billing amount.
    TotalCharges – Total charges incurred during the customer’s tenure.
    Churn – Shows whether the customer has discontinued the service (Yes/No).
EDA Summary:
    There are around 7000 data
    Missing Values: 11 Missing values in the Total charges
    Churn rate = 26%
    Churning is high for the following categories:
        Those who have fiber optics
        Thos who dont have internet security
        Those who dont have online backup
        Those who didnt take take any device protection
        Those who are paying on month-to-month basis via eletronic cheque
    Numeric Features: Tenure has two peak, Monthly charges and total charges are right skewed

2. Model used: 
    A. Random Forest Classification
    B. Gradient Boost Classification
    C. XGBooost Classification

3. Inference
XGBoost performed slightly better than other classification models

