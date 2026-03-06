# Banking Customer Insights and Retention
# Project Overview
Customer retention is a critical challenge in the banking industry. This project analyzes customer behavioral and financial data to identify patterns leading to customer churn and build predictive models that help businesses retain valuable customers.

# Business Problem
Customer churn is a major challenge in the banking industry. Retaining existing customers is significantly cheaper than acquiring new ones. This project analyzes banking customer data to identify factors contributing to customer churn and builds predictive models to identify high-risk customers.

# Project Objectives
The objective of this project is to analyze customer behavioral patterns and build predictive models that identify customers likely to churn, enabling banks to take proactive retention measures.

# Dataset Description
The dataset simulates banking customer information and financial attributes. It includes demographic details, financial behavior, and product usage metrics.

Dataset Size
Large synthetic dataset generated using Python to simulate real banking customer data.

Customer Information
| Feature        | Description                             |
| -------------- | --------------------------------------- |
| Customer ID    | Customer unique code                    |
| Customer Name  | Name                                    |
| Gender         | Customer gender                         |
| Age            | Customer Age                            |
| City           | Customer's city name                    |
| Phone number   | Customer's mobile number                |

Financial Attributes
| Feature         | Description                             |
| --------------- | --------------------------------------- |
| Credit Score    | Customer creditworthiness               |
| Account Balance | Account balance                         |
| Estimated Salary| Salary                                  |

Banking Behavior
| Feature              | Description                             |
| -------------------- | --------------------------------------- |
| NumOfProducts        | Number of bank products used            |
| Active Member Status | Whether customer actively uses services |
| Last Transaction Days| Last Transacted Date                    |

Service Interaction
| Feature         | Description                             |
| --------------- | --------------------------------------- |
| Complaint Status| Previous complaint status               |
| Product Type    | Type of Product used by customer        |

Target Variable
| Feature         | Description                                 |
| --------------- | ------------------------------------------- |
| Churn           |  0 = Customer Retained, 1 = Customer Churned|

# Project Workflow
      Data Generation
            ↓
      Data Cleaning
            ↓
      Exploratory Data Analysis
            ↓
      Feature Engineering
            ↓
      Machine Learning Model
            ↓
      Dashboard Visualization

# Exploratory Data Analysis (EDA)
Key Insights
1. Most churned customers have CreditScore below 650
2. Customers with more than 2 complaints show >50% churn rate
3. Churn rate is low for Active customers and multi-product holders
4. South and West regions show higher retention rates

# Machine Learning Model
1. Logistic Regression - Used as a baseline classification model for churn prediction.
2. Random Forest Classifier - Used to capture non-linear relationships and improve prediction accuracy.
Model Evaluation Metrics
| Model               | Accuracy | Precision | Recall | F1   |
| ------------------- | -------- | --------- | ------ | ---- |
| Logistic Regression | 0.75     | 0.40      | 0.53   | 0.46 |
| Random Forest       | 0.80     | 0.35      | 0.52   | 0.42 |

# Feature Importance
Top features influencing churn
1. ActiveStatus
2. CreditScore
3. Salary

# Customer Segmentation
| Segment | Description                 |
| ------- | --------------------------- |
| 0       | Medium balance customers    |
| 1       | Low balance low income      |
| 2       | Low balance high income     |
| 3       | High salary high balance    |

# Dashboard
The dashboard provides insights into customer behavior and churn patterns including:

- Customer distribution by geography
- Credit score vs churn relationship
- Product usage patterns
- Churn by Age Group

# Key Insights
Some important insights from the analysis include:
1. Customers with lower credit scores show a higher churn probability.
2. Customers with fewer products are more likely to leave the bank.
3. Inactive customers have significantly higher churn rates.
4. Certain cities show higher churn concentrations.
5. Customers with low engagement and infrequent transactions have higher churn risk.

# Business Recommendations
Based on the analysis, the following strategies can improve customer retention:
1. Target high-risk customers with personalized offers.
2. Encourage customers to use multiple banking products.
3. Improve engagement with inactive customers.
4. Provide financial advisory support for low credit score customers.
5. Monitor churn probability regularly using predictive models.

# Future Improvements
Possible improvements to extend the project:
- Deploy model using Streamlit
- Add XGBoost model
- Create automated churn monitoring pipeline
