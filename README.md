# Customer Segmentation with K-Means  
## Grouping customers based on spending and credit behavior

This project applies the K-Means algorithm to a credit card customer dataset in order to segment individuals according to their spending, payment habits, credit usage, and engagement. This segmentation helps guide business strategies for marketing, retention, and revenue growth.

---

## Tools & Technologies

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn

---

## Dataset

The dataset is publicly available at [Kaggle – Credit Card Dataset for Clustering](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata)

Contains anonymized customer data, including:  
- Spending behavior  
- Cash advance usage  
- Credit limit  
- Frequency of purchases  
- Payments and repayment behavior

---

## Executive Summary

This K-Means clustering project grouped credit card customers into four different profiles based on how they spend, pay, and use credit. Each cluster reveals patterns that can help guide smarter marketing, CRM, and risk strategies.

**Cluster 0** includes 13% of customers who spend little but rely **heavily on cash advances, and rarely pay off their full balance.** Their behavior indicates financial stress or misuse of credit. For this group, financial education, credit health content, and safer product alternatives could reduce risk and support more responsible usage.

**Cluster 1,** representing 37% of customers, includes **highly consistent and responsible users.** They make frequent purchases, pay reliably, and have balanced usage patterns. These customers are already strong contributors and should continue to receive attention through loyalty programs, cross-selling opportunities, and value-building offers to increase their lifetime value.

**Cluster 2 is the smallest segment** (around 4%), but likely the **most valuable.** These high spenders have large credit limits and a  high purchase frequency. The focus here should be on retention, offering personalized experiences and premium service to keep them engaged.

**Cluster 3 stands out as the largest segment,** making up 45% of the customer base. These customers show low card usage, low balances, and limited engagement overall. While they don’t contribute much revenue today, their size means even a small improvement in this group could generate significant impact. This cluster should be explored further. Incentive-driven campaigns, lifecycle emails, or entry-level credit benefits might be effective first steps.

**Key Actions**
*   Deep dive into Cluster 3: This group holds untapped potential due to its size. Further segmentation and testing should be prioritized to find paths to reactivation.
*   Maintain and grow Clusters 1 and 2: These are already valuable. Focus on increasing engagement and loyalty through personalized campaigns.
*   Mitigate risk in Cluster 0: Address credit stress with targeted content and safer credit offerings.

---

## Project Worfklow

1. **Data loading and exploration**  
Read the dataset `CC GENERAL.csv`, inspect null values and variable structure.

2. **Data cleaning and preparation**  
Removed the `CUST_ID` column and handled nulls. Data was scaled using `StandardScaler`.

3. **Finding optimal number of clusters (Elbow Method)**  
Used Within-Cluster Sum of Squares (WCSS) to determine the ideal number of clusters (4).

![image](https://github.com/user-attachments/assets/e8739780-4573-43b0-b397-9a8fad179e06)

4. **Running K-Means algorithm**  
Grouped customers into 4 distinct clusters.

6. **Cluster visualization using PCA**  
Reduced dimensionality for 2D plotting of clusters using Principal Component Analysis.

![image](https://github.com/user-attachments/assets/c8b6ef07-6294-4cc3-92a3-a40e3f2214c9)

6. **Cluster behavior profiling**  
Analyzed average behavior of each cluster across key variables.

![image](https://github.com/user-attachments/assets/f9cea010-6b2b-464c-a315-636afec2071a)

![image](https://github.com/user-attachments/assets/f790af5d-277f-45a0-94e0-3599c523fb1a)

![image](https://github.com/user-attachments/assets/c9285bff-99b5-4372-b0a8-796f6f11c981)
