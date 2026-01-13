# TelecomX

Project Overview

I have been hired as a Data Analysis Assistant at Telecom X for the "Customer Churn" project. The goal is to address high cancellation rates by identifying the key drivers of customer loss.

Using Python, I am responsible for the end-to-end data workflow—from collection to analysis—providing the foundation for the Data Science team to build predictive models and retention strategies.

What I will practice:

-API Integration: Efficient data import and manipulation.
-ETL Pipeline: Applying Extract, Transform, and Load concepts.
-Data Visualization: Building strategic charts to spot trends.
-EDA: Performing Exploratory Data Analysis and reporting insights.

Introduction

Customer churn is one of the primary challenges faced by telecommunications companies, as it directly impacts revenue and Customer Acquisition Costs (CAC). The objective of this analysis is to identify patterns and factors associated with customer cancellation using historical data from **Telecom X**.

Through Exploratory Data Analysis (EDA), I sought to understand the profile of customers most likely to churn and generate insights to support churn reduction and strategic decision-making.

---

Data Cleaning and Preprocessing

Initially, the data was imported into a **Google Colab** environment and underwent a cleaning and treatment process, including:

* **Handling Missing Values:** Identification and treatment of null entries.
* **Categorical Encoding:** Converting categorical variables into suitable formats for analysis.
* **Standardization:** Transforming the "Churn" column (Yes/No) into numerical representations (1 and 0).
* **Feature Engineering:** Creation of the `daily_charges` variable, derived from monthly values, to enrich the analysis.
* **Data Integrity:** Verification of data types and information consistency.

These steps ensured high reliability and quality for the subsequent analysis.

---

Exploratory Data Analysis (EDA)

During the exploratory phase, data visualizations were used to identify patterns and relationships between variables and customer churn.

* **Tenure (Contract Time) vs. Churn:** Boxplots revealed that customers who churned tended to have shorter tenures, indicating that cancellation occurs most frequently in the early months of the relationship with the company.
* **Monthly Charges vs. Churn:** The distribution of monthly charges showed that customers with higher bills have a higher propensity to churn, suggesting **price sensitivity**.
* **Total Charges vs. Churn:** It was observed that active customers have significantly higher total charges, which is expected as they remain in the database longer.
* **Contract Type vs. Churn:** Month-to-month contracts showed a much higher churn rate compared to one-year or two-year contracts, indicating lower customer loyalty in short-term agreements.
* **Payment Method vs. Churn:** Customers using **Electronic Checks** had a higher churn rate compared to automatic methods (Credit Card or Bank Transfer), suggesting that payment automation may contribute to retention.
* **Gender vs. Churn:** The analysis by gender showed that churn occurs relatively equally between men and women, indicating that gender alone is not a determining factor.
* **Correlation Analysis:** The correlation matrix indicated a moderate positive correlation between `monthly_charges`, `daily_charges`, and `total_charges`. A negative correlation was found between `total_charges` and `churn`, reinforcing that long-term, more engaged customers churn less.

---

Conclusions and Insights

The analysis identified key factors associated with customer churn:

1. **Early Churn:** Customers with short contract tenures are more likely to leave.
2. **Pricing Pressure:** High monthly charges increase the probability of cancellation.
3. **Contractual Weakness:** Month-to-month contracts have the highest turnover rates.
4. **Service Portfolio:** The absence of additional services is related to higher churn.
5. **Engagement:** Highly engaged customers with higher accumulated spend tend to stay.
6. **Payment Friction:** The payment method has a strong relationship with churn; electronic checks see higher attrition while automatic methods see higher retention.

---

Recommendations

Based on the insights gathered, the following actions are recommended:

* **Onboarding Retention:** Create specific retention strategies for the first few months of a contract, such as "welcome" offers.
* **Price Optimization:** Offer discounts or personalized plans for high-value customers showing signs of dissatisfaction.
* **Contract Migration:** Incentivize customers to migrate from month-to-month plans to long-term contracts.
* **Value Addition:** Promote bundles with additional services to increase the perceived value of the subscription.
* **Automation Incentives:** Encourage the use of automatic payment methods to reduce friction and accidental churn.
* **Predictive Modeling:** Use this cleaned dataset as a foundation for developing future churn prediction machine learning models.

Final Considerations

This analysis demonstrates how data and visualization can support strategic decisions to reduce customer attrition. The insights obtained provide a solid foundation for retention actions and more advanced predictive analytics in the future.
