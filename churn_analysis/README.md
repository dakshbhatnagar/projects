# Customer Churn Analysis

## Overview
This project aims to analyze customer churn in the financial sector, focusing on understanding the factors contributing to customer exits. 

![image](https://www.cleartouch.in/wp-content/uploads/2022/11/Customer-Churn.png)

The analysis highlights key demographics, credit scores, and product engagement levels, providing actionable insights for retention strategies.

## Executive Summary

This analysis of customer churn reveals critical insights into the factors influencing customer retention and attrition:

- **Churn Rate**: Approximately 20% of customers experience churn, indicating a significant area for improvement in customer retention strategies.
- **Credit Score Trends**: The distribution of credit scores is left-skewed, with a mean of 650, suggesting a concentration of customers with lower creditworthiness.
- **Geographic Insights**: France has the highest churn rates, followed by Germany and Spain, highlighting a regional issue that requires targeted interventions.
- **Demographic Factors**: Female customers in France exhibit the highest churn rates, particularly those aged 35-55, indicating a need for tailored engagement strategies for this demographic.
- **Tenure Analysis**: Customers with a tenure of 9-10 years are at the highest risk of churn, suggesting that long-term loyalty does not guarantee retention.
- **Product Offering**: Many long-tenured customers with average or good credit scores hold only one product, indicating potential dissatisfaction with product offerings and a need for diversification.
- **Key Predictors**: Age and account balance are the most significant predictors of churn, while other factors show weak or negative correlations.
- **Early Churn Risk**: Customers with poor credit scores exhibit a high churn rate of 46% within the first four years, escalating to 63% by the sixth year, necessitating early intervention strategies.
- **Inactive Members**: Inactive members have a churn rate of 13%, underscoring the importance of engagement initiatives to retain these customers.

## Key Insights

- **Churn Rate**: 20% of customers are churned, while 80% remain loyal.
- **Credit Score Distribution**: The average credit score of churned customers shows a left-skewed histogram with a mean of 650.
- **Geographical Analysis**: France has the highest churn rate, followed by Germany and Spain.

![image](/churn_analysis/output.png)

- **Demographic Trends**: 
  - French females exhibit the highest churn rates, particularly those aged 35-55.
  - Customers with a tenure of 9-10 years are most likely to churn in France.
  - Male customers have a churn rate of 43% within the age range of 40-45.
- **Customer Segmentation**: 
  - The majority of churned customers (tenure 9-10) have an Average (40.44%) or Good (32.35%) credit score, indicating a higher churn risk among typically low-risk customers.
  - Long-tenured customers with only one product are more prone to churn, suggesting a need for product upgrades or diversification.
- **Feature Correlation**: Age and account balance show the strongest correlation with churn, while other factors demonstrate weak or negative correlations.
- **Churn Rates Over Time**: In the first four years, customers with a poor credit score experience a churn rate of 46%, which increases to 63% by the sixth year.
- **Member Engagement**: Inactive members show a 13% churn rate, indicating a need for engagement through schemes or new product offerings.

## Recommendations

1. **Targeted Engagement for Female Customers**: Given that female customers in France, particularly those aged 35-55, exhibit the highest churn rates, it is crucial to develop tailored engagement strategies. This could include personalized communication, targeted marketing campaigns, and surveys to understand their specific needs and pain points.

2. **Product Diversification for Long-Tenured Customers**: Many long-tenured customers with average or good credit scores hold only one product. To address potential dissatisfaction, consider expanding product offerings or enhancing existing products to better meet the evolving needs of these customers. Introducing loyalty programs or bundling services could also encourage retention.

3. **Early Intervention for Poor Credit Score Customers**: With a significant churn rate of 46% within the first four years for customers with poor credit scores, implementing early intervention strategies is essential. This could involve offering financial education, personalized support, or incentives to improve their credit scores, thereby increasing their likelihood of remaining customers.

4. **Re-engagement Strategies for Inactive Members**: Inactive members have a higher churn rate of 13%. To mitigate this, develop re-engagement strategies such as personalized offers, targeted promotions, or showcasing new products. Regular communication and feedback mechanisms can help keep these customers engaged and reduce the risk of churn.

## Conclusion
This analysis reveals critical insights into customer behavior and highlights potential areas for improving customer retention. By understanding the factors that lead to churn, companies can implement targeted strategies to engage customers more effectively and reduce attrition rates.

## Future Work
- Implement targeted retention campaigns based on customer demographics and behavior.
- Conduct further analysis on product features to identify opportunities for innovation and improvement.

## Installation

To run the project locally, open up the code editor of your choice and move to the terminal. Then follow the instructions below:-

1. Clone the repository:

   ```bash
   git clone https://github.com/dakshbhatnagar/projects/churn_analysis.git
   ```

2. Switch to the directory:
   ```bash
   cd churn_analysis
   ```

You can now start browsing files and exploring data locally on your machine.
   
---
## Usage

Navigate to and open the [Jupyter Notebook](/churn_analysis/Churn.ipynb) files to view detailed analysis, code, and visualizations.
