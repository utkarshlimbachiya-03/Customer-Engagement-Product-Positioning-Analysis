# Customer-Engagement-Product-Positioning-Analysis

**Business Problem:**


How is customer engagement distributed across product categories, and does pricing align with customer satisfaction?

This analysis evaluates:

•	Engagement concentration across categories

•	Premium pricing effectiveness

•	Discount impact on engagement

•	Product performance segmentation

**Dataset Overview:**


Link: https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset

The initial dataset contained product-level and review-level attributes, including pricing, ratings, discount information, and customer review metadata.

Although the dataset contained both product and review-level information, this analysis focused on:

•	Pricing variables

•	Rating & rating-count

•	Category hierarchy

Textual review fields and identifiers were excluded from structured pricing and engagement analysis to reduce dimensionality and maintain analytical focus.

Features Used for Analysis:

•	Actual-price

•	Discounted-price (Final Price)

•	Discount-percentage

•	Rating

•	Rating-count (used as engagement proxy)

•	Category (engineered into hierarchical levels: Department-Category-Sub-Category, Sub-sub-Category, Product type)

•	Product-ID (Actual total products)


**Tech Stack:**

•	Python (Pandas, NumPy, Matplotlib)

•	SQL(SQLite- Aggregations, CTEs, Window Functions)

•	Power BI (KPI dashboard & drill-down analysis)


**Analytical Approach:**

Data Preparation:

•	Numeric standardisation

•	Hierarchical category feature engineering

•	Conditional imputation for missing values

Exploratory Analysis:

•	Distribution & skewness analysis

•	Outlier detection (IQR)

•	Pearson & Spearman correlation testing

SQL-Based Aggregation:

•	Engagement share calculation

•	Top 3 concentration ratio

•	Price segmentation (Budget / Mid / Premium)

•	Performance segmentation (Star, Hidden Gem, Low Performer)

Dashboard Development:

•	Total engagement

•	Weighted average rating

•	Engagement-weighted revenue proxy

•	Price-rating positioning map


**Key Findings:**

•	The top 3 categories generate 53% of total engagement.

•	60% of premium-priced products fall into the low-performance segments.

•	Correlation analysis (Pearson & Spearman) revealed a weak relationship between discount percentage and engagement, raising questions about promotional efficiency.

•	Some products get high engagement but low ratings or vice-versa, which may indicate quality issues.


**Observation Screenshots**

Finding 1:
<img width="849" height="203" alt="image" src="https://github.com/user-attachments/assets/bf404e83-ef19-4598-a6b0-5ba56d406511" />

Finding 2:
<img width="1600" height="601" alt="image" src="https://github.com/user-attachments/assets/3a23c031-c73a-4be3-b0ce-3c3e5ee491e6" />

Findng 3:
Spearman matrix

<img width="768" height="659" alt="image" src="https://github.com/user-attachments/assets/f9516ab4-cd98-4b99-a119-b63b1e163fff" />

Pearson Matrix

<img width="768" height="659" alt="image" src="https://github.com/user-attachments/assets/b9d1fe38-0032-49f1-b245-0b4a775c6d7b" />

Finding 4:

<img width="1600" height="601" alt="image" src="https://github.com/user-attachments/assets/54773253-c7d9-428d-acba-eafd09469927" />


**Recommendations**

•	Inclusion of actual revenue to understand the product performance more accurately.

•	Prioritise quality improvement in high-visibility segments.

•	Improve data collection with actual sales metrics.


**Business Impact**

This project demonstrates:

•	Engagement concentration analysis

•	Pricing elasticity evaluation

•	KPI-driven dashboard development

•	Translation of statistical findings into strategic recommendations



