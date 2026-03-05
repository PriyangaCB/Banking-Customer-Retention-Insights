# Banking Customer Insights and Retention
# Project Overview
Customer retention is a critical challenge in the banking industry. Retaining existing customers is significantly more cost-effective than acquiring new ones. This project focuses on analyzing customer data to identify patterns that lead to customer churn and provide actionable insights that help banks improve retention strategies.
This end-to-end analytics project covers the complete data science workflow including data generation, data preprocessing, exploratory data analysis and predictive modeling.

# Business Problem
Banks often face customer churn due to factors such as poor engagement, low product usage, or dissatisfaction with services. Identifying customers who are likely to leave the bank allows businesses to take proactive steps such as targeted offers or improved customer support.

This project aims to answer the following questions:
- Which customer segments are more likely to churn?
- How do financial attributes influence customer retention?
- Which products have the highest churn rates?
- What behavioral patterns indicate a high churn risk?
- How can businesses identify high-risk customers early?

# Project Objectives
The primary objectives of this project are:
1. Build a realistic banking dataset for analytical modeling.
2. Perform data cleaning and preprocessing.
3. Conduct exploratory data analysis to identify key patterns.
4. Develop machine learning models to predict customer churn.
5. Compare different algorithms for prediction performance.
6. Provide recommendations to improve customer retention.

# Dataset Description
The dataset simulates banking customer information and financial attributes. It includes demographic details, financial behavior, and product usage metrics.

Dataset Size
Large synthetic dataset generated using Python to simulate real banking customer data.

Key Features
Customer Information
- Customer ID
- Customer Name
- Gender
- Age
- City
- Phone Number

Financial Attributes
- Credit Score
- Account Balance
- Estimated Salary

Banking Behavior
- Number of Products
- Active Member Status
- Last Transaction Days

Service Interaction
- Complaint Status
- Product Type

Target Variable
- Churn (0 = Customer Retained, 1 = Customer Churned)

# Tools & Technologies
The project was implemented using the following tools:
Programming - Python
Python Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

Development Environment
- Google Colab / Jupyter Notebook

Version Control
- GitHub

# Project Workflow
1. Data Generation
A large synthetic dataset was generated using Python to simulate real banking customer behavior. This includes generating realistic customer demographics, financial attributes, and transactional behavior.
Key steps:
- Random generation of customer IDs
- Gender-consistent names
- Indian city names
- Phone numbers starting with +91
- Credit score-based active membership logic

2. Data Cleaning & Preprocessing
Data preprocessing was performed to ensure the dataset was suitable for analysis and machine learning.
Key steps included:
- Handling missing values
- Removing duplicates
- Converting data types
- Encoding categorical variables
- Feature engineering
New derived features were created where necessary to improve model performance.

3. Exploratory Data Analysis (EDA)
Exploratory analysis was conducted to understand relationships between customer attributes and churn behavior.
Key analysis performed:
- Customer distribution by gender and city
- Credit score distribution
- Balance vs churn analysis
- Product usage vs churn rate
- Active members vs inactive members
- Customer age trends

Visualization tools used:
- Matplotlib
- Seaborn

4. Churn Prediction Modeling
Machine learning models were built to predict the probability of customer churn.
Algorithms Used
1. Logistic Regression - Used as a baseline classification model for churn prediction.
2. Random Forest Classifier - Used to capture non-linear relationships and improve prediction accuracy.
Model Evaluation Metrics
The models were evaluated using the following metrics:
- Accuracy
- Precision
- Recall
- F1 Score
Example performance:
Logistic Regression
Accuracy: ~0.74
Precision: ~0.40
Recall: ~0.53
F1 Score: ~0.46

Random Forest
Accuracy: ~0.80
These models help identify customers with high churn risk based on their behavioral and financial patterns.

# Key Insights
Some important insights from the analysis include:
- Customers with lower credit scores show a higher churn probability.
- Customers with fewer products are more likely to leave the bank.
- Inactive customers have significantly higher churn rates.
- Certain cities show higher churn concentrations.
- Customers with low engagement and infrequent transactions have higher churn risk.

# Business Recommendations
Based on the analysis, the following strategies can improve customer retention:
1. Target high-risk customers with personalized offers.
2. Encourage customers to use multiple banking products.
3. Improve engagement with inactive customers.
4. Provide financial advisory support for low credit score customers.
5. Monitor churn probability regularly using predictive models.

# Project Structure
banking-customer-insights-retention
data
- churn-data.csv
- customers.csv
- transactions.csv
- bank-customer-master.csv
- bank-churn-prediction.csv

notebooks
- generate-data.ipynb
- load-data.ipynb
- data_analysis.ipynb
- churn_prediction_model.ipynb

# Future Improvements
Possible improvements to extend the project:
- Add more machine learning models such as XGBoost
- Implement hyperparameter tuning
- Deploy the model using Streamlit
- Create real-time churn prediction APIs
- Integrate SQL database pipelines
- Built interactive Excel and Tableau Dashboard to understand the analysis in a better way
