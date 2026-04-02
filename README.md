# cohort-analysis-python
This project performs an in-depth cohort analysis to understand customer behavior over time. It calculates retention rates, churn rates, and average revenue per user (ARPU), providing actionable insights into customer loyalty and engagement. Both weekly and monthly cohorts are analyzed to uncover trends in repeat purchases and revenue.

![](/picture/cohort.png)

## Dataset

The dataset contains e-commerce transactions with the following columns:

- `Invoice` / `order_id` – unique identifier for each order  
- `StockCode` / `product_id` – product identifier  
- `Description` – product name  
- `Quantity` – number of items purchased  
- `InvoiceDate` / `order_date` – purchase timestamp  
- `Price` – unit price  
- `Customer ID` / `customer_id` – unique customer identifier  
- `Country` – customer location  

#### Download the dataset [here](/dataset/year_2009-2010.csv)

## Methodology

### Data Cleaning & Preparation
- Remove duplicates  
- Standardize column names  
- Convert dates and numeric fields  

### Cohort Creation
- Identify **first purchase date** per customer  
- Group customers by **first purchase month/week**  

### Cohort Analysis Metrics
- **Retention Rate** – % of customers returning after first purchase  
- **Churn Rate** – % of customers lost over time  
- **Revenue per User (ARPU)** – average revenue generated per customer  

### Visualization
- Pivot tables for **cohort lifetime**  
- Heatmaps to highlight **retention** and **revenue trends**  

#### Explore the notebook [here](/code/cohort_analysis.ipynb)