# 📊 Customer Churn Prediction using RFM Analysis & Machine Learning

## 📌 Project Overview

This project analyzes customer transaction data from an online retail company to understand purchasing behaviour, identify valuable customer segments, and classify customers based on their churn status.

Using **Exploratory Data Analysis (EDA)**, **Recency-Frequency-Monetary (RFM) Analysis**, and **Machine Learning**, the project transforms retail transaction data into meaningful customer insights.

The objective is to understand customer purchasing patterns, identify high-value customers, analyze customer inactivity, and develop classification models that support customer retention strategies.

---

# ⭐ STAR Methodology

## 🟢 Situation

Customer retention is an important challenge in the retail industry. Businesses collect large volumes of transaction data but need effective ways to understand customer purchasing behaviour, identify valuable customers, and recognize inactive customers.

This project uses the **Online Retail II Dataset** to analyze customer transactions and develop a customer churn classification model.

### Dataset Information

- Dataset: Online Retail II
- Total Transactions: 525,461
- Total Columns: 8
- Customer-level Records: 4,383

### Dataset Attributes

- Invoice Number
- Stock Code
- Product Description
- Quantity Purchased
- Unit Price
- Invoice Date
- Customer ID
- Country

## 🎯 Task

The main objectives of this project were to:

- Perform Exploratory Data Analysis (EDA) to understand customer purchasing behaviour.
- Identify monthly revenue trends and geographic sales distribution.
- Analyze customer revenue contribution and purchase frequency.
- Segment customers using RFM Analysis.
- Define customer churn using a 90-day inactivity threshold.
- Develop machine learning classification models.
- Evaluate model performance using classification metrics.
- Generate business recommendations to support customer retention.

---

## ⚙️ Action

### 1. Data Loading and Quality Audit

Loaded the Online Retail II dataset using Python and Pandas.

Performed an initial data quality audit to examine:

- Dataset dimensions and data types.
- Missing values in customer and product information.
- Duplicate transaction records.
- Negative and zero quantities.
- Negative and zero product prices.

### 2. Data Preparation and Feature Creation

- Created a Revenue column using Quantity × Price.
- Converted InvoiceDate into datetime format.
- Extracted Year-Month for monthly revenue analysis.
- Aggregated transaction data at the customer level.
- Calculated total revenue, total orders, average order value, and unique products purchased.

### 3. Exploratory Data Analysis (EDA)

Performed analysis across the following areas:

- Monthly Revenue Trends
- Revenue Contribution by Country
- Top 20 Products by Revenue
- Customer Revenue Distribution
- Customer Purchase Frequency
- Average Order Value (AOV)
- Unique Products Purchased
- Top 10% Customer Revenue Contribution

### 🔍 Top EDA Findings

#### 1️⃣ Revenue Concentration Among High-Value Customers

**Observation:**

The top 10% of customers generated significantly higher average revenue than the remaining customers.

| Customer Group | Average Revenue | Average Orders |
|---|---:|---:|
| Top 10% Customers | 11,518.08 | 21.12 |
| Other Customers | 834.63 | 3.63 |

**Business Takeaway:**

- Prioritize high-value customer retention.
- Introduce loyalty rewards.
- Provide exclusive promotions.
- Develop personalized marketing campaigns.

#### 2️⃣ Monthly Revenue Trends

**Observation:**

Monthly revenue analysis showed fluctuations across the dataset period.

- Highest Revenue Month: November 2010
- Revenue: 1,422,654.64
- Lowest Revenue Month: December 2010
- Revenue: 377,488.45

**Business Takeaway:**

- Plan promotional campaigns strategically.
- Improve inventory planning.
- Analyze seasonal demand patterns.
- Optimize marketing activities.

#### 3️⃣ Geographic Revenue Concentration

**Observation:**

The United Kingdom contributed the largest share of revenue.

| Country | Revenue |
|---|---:|
| United Kingdom | 8,194,777.53 |
| EIRE | 352,242.73 |
| Netherlands | 263,863.41 |
| Germany | 196,290.35 |
| France | 130,769.90 |

**Business Takeaway:**

- Focus on high-performing geographic markets.
- Identify opportunities in other countries.
- Develop region-specific marketing strategies.

#### 4️⃣ Customer Purchasing Behaviour

**Observation:**

Customer-level analysis was performed using:

- Total Revenue
- Total Orders
- Average Order Value
- Unique Products Purchased

The analysis helps identify differences between frequent buyers, occasional buyers, and high-value customers.

**Business Takeaway:**

- Encourage repeat purchases.
- Introduce customer loyalty programs.
- Recommend relevant products.
- Improve cross-selling opportunities.

---

## 📊 RFM Customer Segmentation

RFM Analysis was applied to understand customer value and purchasing behaviour.

RFM stands for:

- **Recency:** How recently a customer made a purchase.
- **Frequency:** How frequently a customer places orders.
- **Monetary:** How much revenue a customer generates.

Customers were assigned scores from 1 to 5 using quintile-based scoring.

### Customer Segments

| Customer Segment | Number of Customers |
|---|---:|
| Champions | 1,096 |
| Loyal | 821 |
| New | 378 |
| At Risk | 713 |
| Lost | 1,375 |
| **Total** | **4,383** |

### Business Takeaway

- **Champions:** Provide exclusive rewards and VIP benefits.
- **Loyal:** Strengthen relationships through loyalty programs.
- **New:** Encourage repeat purchases through onboarding offers.
- **At Risk:** Launch personalized re-engagement campaigns.
- **Lost:** Use targeted win-back offers.

---

## 🤖 Machine Learning – Customer Churn Prediction

### 1. Problem Definition

Customer churn was defined using a **90-day inactivity threshold**.

- `1 = Churned Customer` — No purchase in more than 90 days.
- `0 = Active Customer` — Purchase within the last 90 days.

### 2. Customer Churn Distribution

| Customer Status | Number of Customers |
|---|---:|
| Active Customers | 2,934 |
| Churned Customers | 1,449 |
| **Total** | **4,383** |

### 3. Feature Engineering

Created a customer-level feature dataset using the following variables:

- Recency
- Frequency
- Monetary
- Average Order Value
- Unique Products
- Average Days Between Purchases
- Return Rate

These features represent customer purchasing activity, spending behaviour, product diversity, and transaction returns.

### 4. Machine Learning Models

Developed two supervised classification models:

- Logistic Regression
- Random Forest Classifier

### 5. Train-Test Split

The dataset was divided into:

- Training Data: 80%
- Testing Data: 20%

Additional preprocessing steps included:

- StandardScaler for feature scaling.
- SimpleImputer for handling missing values through mean imputation.

---

## 📈 Model Evaluation

The models were evaluated using the following classification metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score
- Confusion Matrix

### Model Performance Results

| Evaluation Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Accuracy | 99.66% | 100.00% |
| Precision | 100.00% | 100.00% |
| Recall | 98.93% | 100.00% |
| F1 Score | 99.46% | 100.00% |
| ROC-AUC | 1.00 | 1.00 |

### 🏆 Model Comparison

Random Forest achieved the highest scores across all reported evaluation metrics.

However, these results require an important qualification:

**Modelling Limitation:** The churn target is created using a 90-day inactivity rule, while Recency is also included as a model input. Since both variables represent almost the same underlying information, this introduces target leakage and can artificially inflate model performance.

Therefore, the reported scores should not be interpreted as proof of real-world predictive accuracy. A more reliable evaluation should exclude the leakage-prone Recency feature or define churn using a future observation period and validate the model using a time-based train-test split.

---

## 🔍 Feature Importance Analysis

Random Forest feature importance was used to understand the variables contributing most to the model's predictions.

| Feature | Importance |
|---|---:|
| Recency | 0.8505 |
| Monetary | 0.0433 |
| Frequency | 0.0372 |
| Unique Products | 0.0326 |
| Avg Days Between Purchases | 0.0208 |
| Average Order Value | 0.0106 |
| Return Rate | 0.0049 |

**Key Observation:** Recency received the highest importance score. This is consistent with the target leakage limitation because the churn label is directly based on customer inactivity.

---

# 📌 Business Recommendations

## 1️⃣ Implement Targeted Customer Retention Campaigns

- Identify customers classified as At Risk.
- Use personalized email campaigns.
- Provide targeted discount coupons.
- Develop re-engagement strategies.

## 2️⃣ Strengthen Customer Loyalty Programs

- Reward Champions and Loyal customers.
- Provide exclusive deals.
- Introduce loyalty benefits.
- Encourage repeat purchases.

## 3️⃣ Optimize Marketing and Product Strategies

- Recommend relevant products.
- Bundle frequently purchased items.
- Improve cross-selling opportunities.
- Increase average order value.

## 4️⃣ Focus on Geographic Markets

- Prioritize high-performing countries.
- Explore opportunities in other markets.
- Develop region-specific promotional campaigns.

---

# 📌 Business Impact

This project demonstrates how customer transaction data can support business decision-making through:

- Customer segmentation and profiling.
- Identification of high-value customers.
- Analysis of customer purchasing behaviour.
- Understanding revenue and geographic trends.
- Identification of inactive customer segments.
- Data-driven customer retention recommendations.

The project provides an analytical foundation for improving customer engagement and developing more reliable churn prediction strategies.

---

# 🛠️ Tech Stack

### Programming Language
- Python

### Data Analysis and Manipulation
- Pandas
- NumPy

### Data Visualization
- Matplotlib
- Seaborn

### Machine Learning
- Scikit-learn
- Logistic Regression
- Random Forest Classifier

### Data Preprocessing
- StandardScaler
- SimpleImputer
- Train-Test Split

### Development Environment
- Jupyter Notebook

---

# 📂 Project Workflow

```text
Business Problem
        |
        ▼
Data Collection
        |
        ▼
Data Loading using Pandas
        |
        ▼
Data Quality Audit
        |
        ▼
Revenue Calculation
        |
        ▼
Exploratory Data Analysis
        |
        ▼
Customer Behaviour Profiling
        |
        ▼
RFM Analysis and Segmentation
        |
        ▼
Churn Target Creation
        |
        ▼
Feature Engineering
        |
        ▼
Data Preprocessing
        |
        ▼
Machine Learning Models
(Logistic Regression & Random Forest)
        |
        ▼
Model Evaluation
        |
        ▼
Feature Importance Analysis
        |
        ▼
Business Insights and Recommendations
```

---

# 📁 Repository Structure

```text
Customer-Intelligence-Project/
│
├── Mba_Project_2502057.ipynb
│
├── MBA_Summary_2502057.pdf
│
├── README.md
│
└── data/
    └── Online_Retail_II.xlsx
```

*Note: The dataset should be placed in the data folder if you choose to organize your repository this way. Update the notebook's dataset path accordingly.*

---

# 🚀 Future Improvements

- Address target leakage and improve churn prediction methodology.
- Apply time-based model validation.
- Experiment with XGBoost and other classification algorithms.
- Develop an interactive customer analytics dashboard using Power BI.
- Deploy the model using Streamlit.
- Build customer-level retention recommendations.

---

# 👨‍💻 Author

**Harendra**

MBA – Business Analytics

Business Analytics | Python | SQL | Machine Learning | Customer Analytics

---

## ⭐ Support

If you find this project useful, please consider giving the repository a ⭐ Star.

Thank you for visiting my project!
