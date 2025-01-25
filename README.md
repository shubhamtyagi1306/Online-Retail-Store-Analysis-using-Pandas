# Online-Retail-Store-Analysis-using-Pandas

## Project Overview
This project is an **end-to-end data analysis project** built using the Pandas library. It analyzes transactional data from an online retail store to gain insights into customer behavior and business trends. The project leverages real-world data to calculate sales trends, identify anomalies, and segment customers based on the **Recency, Frequency, and Monetary (RFM)** model. 

The insights derived from this project can be used for targeted marketing, customer retention strategies, and improving overall business performance.

---

## Dataset Information
The dataset used in this project contains transactions from an online retail store. Each row represents an individual invoice item, including:
- **InvoiceNo**: Unique identifier for the transaction.
- **StockCode**: Unique identifier for the product.
- **Description**: Product description.
- **Quantity**: Number of products purchased.
- **InvoiceDate**: Date and time of the transaction.
- **UnitPrice**: Price per unit of the product.
- **CustomerID**: Unique identifier for the customer.
- **Country**: Country of the customer.

### Download the Dataset
You can download the dataset from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Online+Retail) or similar publicly available sources.

---

## Steps Performed

### 1. **Data Cleaning**
- Handled missing values in critical columns (e.g., removed rows with missing `CustomerID`).
- Filtered out transactions with negative quantities.
- Converted `InvoiceDate` to datetime format for time-based analysis.

### 2. **Exploratory Data Analysis (EDA)**
- Calculated total sales by adding a `TotalPrice` column (`Quantity * UnitPrice`).
- Identified sales trends by grouping transactions monthly.
- Visualized trends using line charts to observe seasonal patterns.

### 3. **RFM Segmentation**
- Defined RFM metrics:
  - **Recency**: Number of days since the customer's last purchase.
  - **Frequency**: Number of transactions made by the customer.
  - **Monetary**: Total amount spent by the customer.
- Grouped and aggregated data by `CustomerID`.
- Scored customers based on RFM metrics using quantiles.
- Created customer segments (e.g., Champions, Loyal Customers, At-Risk Customers).

### 4. **Visualization and Insights**
- Plotted sales trends, customer distribution, and revenue contribution by segment.
- Highlighted high-value customers and opportunities for targeted marketing.

---

## Key Findings
1. **Top-Performing Months**: Identified months with the highest sales volume.
2. **High-Value Customers**: Defined and targeted Champions for loyalty rewards.
3. **Customer Retention**: Highlighted at-risk customers for re-engagement campaigns.
4. **Anomalies**: Detected and removed erroneous data (e.g., negative transactions).

---

## Tools and Libraries Used
- **Python**
  - `pandas`: Data manipulation and analysis
  - `matplotlib` & `seaborn`: Data visualization
- **Jupyter Notebook**: Development environment

---

## Applications
- **Marketing Campaigns**: Implement targeted campaigns based on customer segmentation.
- **Business Strategy**: Identify high-value customers and optimize resource allocation.
- **Forecasting**: Predict future sales trends using time-series analysis.

---

## How to Run the Project
1. Clone the repository to your local machine.
2. Install the required Python libraries:
   ```bash
   pip install pandas matplotlib seaborn
   ```
3. Download the dataset and place it in the `data/` directory.
4. Run the Jupyter Notebook to execute the analysis.

---

## Future Enhancements
- Implement machine learning models for customer churn prediction.
- Automate anomaly detection and data cleaning.
- Build an interactive dashboard for real-time monitoring of sales and customer metrics.

---

## Author
This project is developed by Shubham Tyagi. If you have any questions or suggestions, feel free to reach out at shubhamtyagi1306@gmail.com.
