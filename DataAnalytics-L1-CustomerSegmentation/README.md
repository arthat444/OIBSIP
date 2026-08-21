Level 1 - Task 2: Customer Segmentation Analysis
Project Overview
This project focuses on customer segmentation using RFM (Recency, Frequency, Monetary) analysis and K-Means clustering.

The objective is to identify distinct customer groups based on their purchasing behaviour and develop targeted marketing strategies for each segment.

Dataset
The Online Retail dataset was used for this analysis.

The dataset contains retail transactions with information including:

Invoice Number
Stock Code
Product Description
Quantity
Invoice Date
Unit Price
Customer ID
Country
After data cleaning, 4,338 unique customers were available for RFM analysis.

Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Google Colab
K-Means Clustering
Methodology
1. Data Cleaning
The dataset was inspected for:

Missing values
Duplicate records
Cancelled transactions
Invalid unit prices
Transactions without CustomerID were removed because customer-level segmentation requires a valid customer identifier.

Duplicate records and cancelled transactions were also removed.

2. RFM Analysis
Three behavioural features were calculated:

Recency: Number of days since the customer's latest purchase
Frequency: Number of unique invoices/purchasing occasions
Monetary: Total amount spent by the customer
3. Feature Standardisation
RFM features were standardised using StandardScaler before applying K-Means clustering.

4. K-Means Clustering
The Elbow Method was used to determine a suitable number of clusters. Four customer segments were selected and K-Means clustering was applied.

Customer Segments
Cluster	Customers	Segment
0	3,054	Regular Customers
1	1,067	At-Risk / Low-Value Customers
2	13	VIP Customers
3	204	Loyal High-Value Customers
Cluster Profiles
Segment	Avg Recency	Avg Frequency	Avg Monetary
Regular Customers	42.70	3.68	1,353.63
At-Risk / Low-Value Customers	247.08	1.55	478.85
VIP Customers	6.38	82.54	127,187.96
Loyal High-Value Customers	14.50	22.33	12,690.50
Key Insights
Regular Customers form the largest customer segment.
A significant group of customers is inactive and has low purchasing frequency.
A very small VIP segment contributes exceptionally high monetary value.
Loyal high-value customers show strong recent engagement and frequent purchasing behaviour.
Marketing Recommendations
Regular Customers
Use loyalty points, personalised recommendations, and repeat-purchase offers to increase customer lifetime value.

At-Risk / Low-Value Customers
Use win-back campaigns, personalised discounts, and reminder emails to encourage customers to return.

VIP Customers
Provide exclusive products, early access, premium support, and personalised VIP offers.

Loyal High-Value Customers
Use loyalty rewards, cross-selling, upselling, and personalised membership benefits to strengthen retention.

Conclusion
RFM analysis combined with K-Means clustering successfully identified four distinct customer segments.

The results demonstrate that customers have substantially different levels of engagement, purchasing frequency, and monetary contribution. Customer segmentation can therefore help businesses replace one-size-fits-all marketing with targeted strategies designed for different customer behaviours.

Files
Customer_Segmentation_RFM_KMeans.ipynb - Complete analysis notebook
customer_segmentation_RFM_results.csv - Final customer segmentation results
