📊 Sales Performance Dashboard – Power BI
This project is a comprehensive Sales Performance Dashboard built using Power BI, designed to analyze and visualize business metrics such as revenue, customer behavior, product performance, and sales trends.

📁 Project Overview
The dashboard provides actionable insights into key sales performance indicators including:

🔹 Total Revenue & Orders

🔹 Average Order Value (AOV)

🔹 Monthly and Weekly Sales Trends

🔹 Product Category Performance

🔹 Customer Segmentation (RFM Analysis)

🔹 Top Performing Customers & Products

🔹 Return & Refund Insights

📌 Key Features
🔹 Sales Summary Page
KPI Cards: Total Revenue, Total Orders, AOV

Monthly Sales Trend (Line Chart)

Top 5 Products by Revenue (Bar Chart)

Revenue by Region/Channel (Map or Treemap)

🔹 Customer Analysis Page
RFM Segmentation (Recency, Frequency, Monetary)

Customer Lifetime Value (CLV)

Demographics: Age Group, Income, No. of Children

Top Customers Highlighted

🔹 Product Insights Page
Revenue by Product Category/Subcategory

Return Rate by Product

Product Performance via Decomposition Tree

🔹 Returns Page
Return Trends by Month

Most Returned Products

Customer Return Behavior

🔹 Information Bookmarks
Highlights key insights using bookmarks and tooltips

E.g., “Lisa Cai, a high-value customer, generated $11.3K in revenue with 7 orders.”

📊 Tools & Technologies
Tool	Usage
Power BI	Data Modeling, Visualization, DAX Measures
DAX	Custom Calculations & KPIs
Power Query	Data Transformation
CSV Files	Data Source

📈 Key DAX Measures
Total Revenue = SUM('Sales'[Price])

Total Orders = COUNTROWS('Sales')

AOV = [Total Revenue] / DISTINCTCOUNT('Sales'[Order ID])

Recency = DATEDIFF(LASTDATE('Sales'[Order Date]), MAX('Sales'[Order Date]), DAY)

Order Target = VAR lastMonth = ... RETURN lastMonth * 1.1

(More DAX measures used for RFM and customer-level KPIs)

📦 Dataset
sales_info.csv – Order data (date, quantity, revenue, etc.)

customer_info.csv – Customer profile (gender, income, age, etc.)

product_info.csv – Product details (category, subcategory, price)

returns_data.csv (optional) – Return records for products

💡 Insights
Here are some key insights derived from the dashboard:

📍 Highest sales were recorded in December, with a 15% increase over the previous month.

👩‍💼 Mrs. Lisa Cai stands out as a top-tier customer, contributing $11.3K in revenue.

📦 Electronics outperform all other categories in both revenue and order volume.

📉 Product returns are highest in Accessories, suggesting quality/fit issues.

👨‍👩‍👧 Customers with 2–3 children show a 20% higher purchase rate.

🖼️ Preview
(Include screenshots or thumbnails of the dashboard pages if possible)

🚀 Getting Started
To explore the dashboard:

Clone this repo

Open Sales performance.pbix in Power BI Desktop

Refresh the data and explore the visualizations

🧠 Learning Outcomes
Built a dynamic, multi-page Power BI dashboard

Applied advanced DAX calculations and relationships

Performed customer segmentation using RFM analysis

Integrated multiple data sources using Power Query

