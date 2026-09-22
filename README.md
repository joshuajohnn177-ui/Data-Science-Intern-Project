# Data-Science-Intern-Project 1

# Customer Segmentation Using K-Means Clustering

## CODTECH Internship Project

### Internship Details

| Details | Information |
|---|---|
| **Name** | Joshua J |
| **Intern ID** | CITS9064 |
| **Domain** | Data Science & Analytics |
| **Internship Duration** | 8 Weeks |
| **Project Name** | Customer Segmentation Using K-Means Clustering |

---

## 1. Project Overview

This project focuses on customer segmentation using the K-Means
clustering algorithm.

The objective is to identify groups of customers with similar
purchasing behaviors and characteristics. Customer segmentation
can help businesses understand different customer groups and
develop more targeted marketing, retention, and engagement
strategies.

The project uses customer purchasing behavior, spending,
discount usage, return activity, and purchase recency to create
behavioral customer segments.

---

## 2. Project Scope

The project covers the following stages:

- Data loading and inspection
- Data cleaning
- Exploratory Data Analysis (EDA)
- Feature correlation analysis
- Feature selection
- Feature standardization
- K-Means clustering
- Elbow and silhouette analysis
- Cluster profiling
- Product preference analysis
- Membership analysis
- Data visualization
- Business interpretation
- Customer segmentation output

---

## 3. Dataset

The dataset contains **500 customer records**.

The dataset includes information related to:

- Customer demographics
- Purchase frequency
- Total purchases
- Total spending
- Average purchase value
- Product categories
- Discount usage
- Return activity
- Days since purchase
- Membership
- Preferred category
- Payment method

The final processed dataset contains **19 columns**, including the
final customer segment assigned by the clustering model.

---

## 4. Technologies Used

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

### Development Environment
- Jupyter Notebook

### Machine Learning Algorithm
- K-Means Clustering

---

## 5. Methodology

The project follows the following workflow:

1. Load the customer dataset
2. Inspect the dataset structure
3. Perform data cleaning
4. Conduct exploratory data analysis
5. Analyze correlations between numerical features
6. Select behavioral features for clustering
7. Standardize the selected features
8. Evaluate different numbers of clusters
9. Compare silhouette scores
10. Build the final K-Means model
11. Profile the resulting customer groups
12. Visualize the customer segments
13. Develop business insights
14. Export the final segmented dataset

---

## 6. Feature Selection

The final K-Means model uses the following behavioral features:

- `Purchase_Frequency`
- `Total_Amount`
- `Discount_Count`
- `Return_Count`
- `Days_Since_Purchase`

These features represent important aspects of customer purchasing
behavior, including frequency, monetary value, discount usage,
return activity, and purchase recency.

The selected features were standardized before applying K-Means.

---

## 7. Model Evaluation

Different values of K were evaluated using the silhouette score.

For the final behavioral feature set, the silhouette scores were
compared for K values from 2 to 10.

The highest score in this evaluation was obtained for:

**K = 5**

Final silhouette score:

**0.291**

The silhouette score indicates that the resulting customer groups
have some meaningful structure while also showing some overlap
between segments.

---

## 8. Final Customer Segments

The final K-Means model created five customer segments.

| Cluster | Customers | Percentage | Segment |
|---|---:|---:|---|
| 0 | 113 | 22.6% | Discount-Oriented Customers |
| 1 | 69 | 13.8% | High-Return Customers |
| 2 | 90 | 18.0% | Inactive Customers |
| 3 | 49 | 9.8% | Premium High-Value Customers |
| 4 | 179 | 35.8% | Regular Customers |

Total customers: **500**

---

## 9. Cluster Characteristics

### Cluster 0 — Discount-Oriented Customers

This segment contains 113 customers.

The group has the highest average discount count and moderate
purchasing activity.

**Key characteristics:**
- 113 customers
- Average purchase frequency: 8.12
- Average total amount: 22,067.17
- Average discount count: 8.42
- Average days since purchase: 96.75

---

### Cluster 1 — High-Return Customers

This segment contains 69 customers.

The distinguishing characteristic of this group is its relatively
high return activity.

**Key characteristics:**
- 69 customers
- Average purchase frequency: 10.28
- Average total amount: 43,677.23
- Average return count: 2.20
- Average days since purchase: 68.03

---

### Cluster 2 — Inactive Customers

This segment contains 90 customers.

It has the lowest purchasing activity and the longest average time
since the previous purchase.

**Key characteristics:**
- 90 customers
- Average purchase frequency: 2.57
- Average total amount: 8,178.82
- Average return count: 0.14
- Average days since purchase: 198.92

---

### Cluster 3 — Premium High-Value Customers

This segment contains 49 customers.

It has the highest purchase frequency and highest average spending,
while also having the shortest average time since purchase.

**Key characteristics:**
- 49 customers
- Average purchase frequency: 18.71
- Average total amount: 134,435.66
- Average discount count: 1.57
- Average days since purchase: 31.76

---

### Cluster 4 — Regular Customers

This is the largest segment, containing 179 customers.

The group demonstrates relatively consistent purchasing activity
and moderate-to-high spending.

**Key characteristics:**
- 179 customers
- Average purchase frequency: 10.75
- Average total amount: 46,521.97
- Average discount count: 3.56
- Average days since purchase: 62.54

---

## 10. Key Findings

The analysis produced several important findings:

1. Cluster 4 is the largest customer segment, representing 35.8%
   of the customer base.

2. Cluster 3 contains 9.8% of customers but has the highest
   average purchase frequency and total spending.

3. Cluster 2 has the lowest purchasing activity and the longest
   average time since purchase.

4. Cluster 0 has the highest average discount usage.

5. Cluster 1 has the highest average return activity.

6. The final K-Means model achieved a silhouette score of 0.291.

---

## 11. Business Applications

The identified customer segments can support different business
strategies.

### Discount-Oriented Customers
- Personalized discounts
- Promotional campaigns
- Bundle offers
- Limited-time offers

### High-Return Customers
- Analyze return reasons
- Improve product information
- Improve size and product guidance
- Recommend suitable products

### Inactive Customers
- Customer reactivation campaigns
- Win-back offers
- Personalized recommendations
- New product notifications

### Premium High-Value Customers
- Loyalty programs
- Exclusive offers
- Early access to products
- Personalized recommendations
- Premium customer engagement

### Regular Customers
- Cross-selling
- Product recommendations
- Loyalty incentives
- Regular engagement campaigns

---

## 12. Project Visualizations

The project includes visualizations for:

- Customer distribution across clusters
- Spending distribution
- Purchase frequency
- Customer recency
- Final customer segmentation
- Silhouette score comparison

All graphs are available in the `outputs/` directory.

---

## 13. Repository Structure

```text
customer-segmentation-kmeans/
│
├── README.md
│
├── notebook/
│   └── Customer_Segmentation_KMeans.ipynb
│
├── data/
│   ├── customer_data.csv
│   └── customer_segmentation_final.csv
│
├── outputs/
│   ├── customer_distribution.png
│   ├── spending_distribution.png
│   ├── purchase_frequency.png
│   ├── customer_recency.png
│   ├── final_customer_segmentation.png
│   └── silhouette_scores.png
│
├── screenshots/
│   ├── notebook_output.png
│   ├── cluster_distribution.png
│   └── final_results.png
│
└── documentation/
    └── Customer_Segmentation_Report.pdf
