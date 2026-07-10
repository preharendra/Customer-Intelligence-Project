# Customer-Intelligence-Project
An end-to-end analytics project combining exploratory data analysis with predictive modelling on a real retail dataset.

# Insight Summary Document 
Problem Statement and Data Used 

This project analyzes customer transaction data from an online retail company 
to understand customer purchasing behavior and identify customers who are 
likely to stop buying from the company. The dataset used for the analysis is the 
Online Retail transaction dataset, which contains information such as invoice 
number, product description, quantity purchased, price per unit, purchase date, 
customer ID, and customer country. The objective of the project was to perform 
exploratory data analysis to understand revenue patterns and customer 
behavior, and then build a predictive model that can identify customers who are 
at risk of churn. By predicting churn early, the business can take proactive 
actions such as targeted marketing campaigns and loyalty programs to retain 
valuable customers. 

Top 5 EDA Findings and Business Takeaways

1. Revenue Concentration Among a Small Group of Customers 
Observation: A relatively small percentage of customers generate a large share 
of total revenue. 
Business Takeaway: The company should prioritize retaining high-value 
customers through loyalty rewards, personalized offers, and exclusive 
promotions.

2. Seasonal Revenue Trends 
Observation: Monthly revenue shows fluctuations, with certain months 
generating significantly higher sales. 
Business Takeaway: The company should plan promotional campaigns and 
targeted marketing during lower-performing months to maintain consistent 
sales.
 
4. Geographic Revenue Concentration 
Observation: A small number of countries contribute the majority of total 
revenue. 
Business Takeaway: Marketing investments should focus on high-performing 
markets while exploring growth opportunities in underperforming regions.
 
5. Customer Purchase Frequency Differences 
Observation: Most customers make only a few purchases, while a smaller group 
of loyal customers purchase frequently. 
Business Takeaway: Encouraging repeat purchases through loyalty programs 
and personalized product recommendations could increase overall revenue.

6. Distinct Customer Segments Identified through RFM Analysis 
Observation: Customers can be grouped into segments such as Champions, 
Loyal, At Risk, and Lost based on purchasing behavior. 
Business Takeaway: Each segment should receive different marketing 
strategies, such as rewards for loyal customers and re-engagement campaigns 
for at-risk customers.

Predictive Model and Evaluation 

To predict customer churn, two machine learning models were trained: Logistic 
Regression and Random Forest. The dataset was split into 80% training data 
and 20% testing data. The models were evaluated using accuracy, precision, 
recall, F1 score, and ROC-AUC metrics. The Random Forest model performed 
better overall, achieving higher predictive performance compared to Logistic 
Regression. The evaluation prioritized the F1 Score and ROC-AUC because 
these metrics provide a balanced measure of the model’s ability to correctly 
identify churned customers while minimizing incorrect predictions.

Business Recommendations 

1. Implement Targeted Customer Retention Campaigns
   
Customers identified as at risk of churn should receive personalized 
promotions, reminder emails, or discount offers to encourage them to return 
and make additional purchases.

3. Strengthen Loyalty Programs for High-Value Customers
   
High-value customers who contribute significantly to revenue should be 
rewarded through loyalty programs, exclusive deals, and early access to new 
products to maintain long-term engagement.

5. Optimize Marketing and Product Strategies Based on Customer Insights
   
Insights from customer purchasing behavior should be used to recommend 
products, bundle popular items, and promote frequently purchased products to 
increase average order value and customer satisfaction.

Overall, the analysis demonstrates that combining customer behavior analytics 
with predictive modeling enables the business to make data-driven decisions 
that improve customer retention, increase revenue, and strengthen long-term 
customer relationships. 
