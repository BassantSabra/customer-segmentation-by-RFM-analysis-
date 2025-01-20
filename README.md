
## **project overview**

- This README provides a step-by-step guide for cleaning and transforming the Excel dataset. The aim is to prepare the data for RFM analysis for customer segmentation 
---

## **Steps for Data Cleaning**

### **1. Remove Unnecessary Columns**
- **Objective**: Simplify the dataset by keeping only the relevant columns.
- **Columns to Keep**:
  - `InvoiceNo`
  - `StockCode`
  - `Description`
  - `Quantity`
  - `InvoiceDate`
  - `UnitPrice`
  - `total_amount`
  - `CustomerID`
  - `Country`

---


### **2. Remove Products with Unit Price equal zero**
- **Objective**: Eliminate invalid transactions where products are listed with a unit price of zero.
- **Steps**:
  - Filter the dataset to find rows where `UnitPrice = 0`.
  - Delete these rows as they likely represent errors or promotional transactions irrelevant to revenue analysis.
- **Action**:
  - Use Excel's `Filter` or a Python script to identify and remove these rows.

### **3. Remove Records without Customer ID**
- **Objective**: Focus only on transactions associated with identifiable customers.
- **Steps**:
  - Filter out rows where `CustomerID` is empty or null.
  - According to your description, approximately 135,000 records fall into this category.
  - Removing these rows will reduce noise and ensure analysis is based on real customer data.

---

## **Steps for RFM analysis and insights**

- By scoring our customers using  RFM analysis ( recency , frequency , monetary), we can identify our 4 major segments for targeting

  
![Screenshot 2025-01-20 210801](https://github.com/user-attachments/assets/f63d4b87-a8f8-4169-acac-127026504da8)


## **1. Top Customer Segment**
- Percentage: 18% of customers fall into this segment.
- Average Spend: These top customers have spent an average of $7,000 in the last 15 days, indicating they are highly engaged and valuable to the business.
## **2. Loyal Customers**
- Percentage: This segment comprises 31.2% of the customer base.
- Importance: Loyal customers are crucial for sustaining revenue, suggesting that maintaining their satisfaction should be a priority.
## **3. At Risk and Need Attention**
- Percentage: 29.5% of customers are categorized as at risk or needing attention.
- Average Spend: At-risk customers have spent only $518, indicating a significant drop in engagement. Strategies should be developed to re-engage these customers.
## **4. Lost Customers**
- Percentage: 20.9% of customers are classified as lost.
- Average Spend: Lost customers spent an average of $179, highlighting a potential revenue loss.

## **recommendations**
- We must create a target campaign to re-engage our At-risk customers and lost customers using personalized email or SMS to offer discounts, limited-time offers to draw them back.

- Use purchase history to recommend products they may find appealing.

- Conduct surveys to understand why they stopped purchasing and implement improvements.

- Ensure consistent communication with customers across all platforms (email, social media, SMS) to maximize reach.

- Launch loyalty programs that offer points or discounts for frequent purchases.

- Regularly share updates, product recommendations, and personalized offers to maintain their engagement.

- Introduce exclusive benefits, such as early access to sales, VIP memberships.










