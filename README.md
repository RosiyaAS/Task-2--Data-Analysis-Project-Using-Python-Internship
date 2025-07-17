# Task-2--Data-Analysis-Project-Using-Python-Internship
This project showcases a complete end-to-end data analysis pipeline using the Global Superstore dataset. The main goal is to clean and prepare the data, extract meaningful insights, engineer useful features, and explore customer and sales trends across markets, regions, and product categories. This notebook is a great example of a real-world business analytics use case and is structured to reflect industry best practices in data science.

📌 Project Objective
The objective of this project is to analyze the Global Superstore dataset to:

Understand sales performance over time

Identify key drivers of profit and revenue

Examine customer behavior and segmentation

Explore the relationship between shipping mode, priority, and fulfillment

Lay the groundwork for future predictive modeling and business optimization

📂 Dataset Description
The dataset used (Global_Superstore.csv) contains transactional data from a global retail operation, including:

Order Information: Order ID, Order Date, Ship Date, Ship Mode

Customer Information: Customer ID, Customer Name, Segment, Country, City

Product Details: Category, Sub-Category, Product Name, Product ID

Sales Metrics: Sales, Quantity, Discount, Profit

Geographic Metadata: Region, Market, Postal Code

🔧 Tools and Technologies Used
Tool/Library	Purpose
pandas	Data manipulation and analysis
numpy	Numerical operations
matplotlib	Data visualization
seaborn	Advanced data visualization
sklearn (optional in later steps)	ML-ready transformation if extended

🔄 Workflow Summary
1. 🛠 Importing Libraries and Dataset
Loaded the dataset using pandas with correct encoding (ISO-8859-1)

Displayed initial rows to understand the structure

2. 🧹 Data Cleaning and Preparation
Converted Order Date and Ship Date to datetime format

Removed supporting split columns after datetime conversion

Categorical fields (Ship Mode, Segment, Category, etc.) were converted to the category data type for efficiency

Cleaned string columns to remove whitespace

Filled missing values:

Used median for numeric columns like Postal Code

Used forward fill for date fields

3. 🔬 Feature Engineering
Created new time-based features such as Order_year

Calculated total Revenue by multiplying Sales and Quantity

Grouped customer data by year to understand customer growth trends

4. 📊 Exploratory Data Analysis (EDA)
Visualized sales, profit, and discount distributions

Identified top-performing regions, markets, and product categories

Investigated shipping trends by analyzing Ship Mode and Order Priority

Generated time series insights to track performance over the years

📈 Insights & Observations
Certain regions and categories contributed significantly to profit, while others resulted in high sales but negative profit due to discounts.

Customer segmentation revealed that "Consumer" and "Corporate" segments were the most active.

Standard Class was the most commonly used shipping mode, while Same Day and First Class were used less frequently.

Sales peaked in specific years and months, offering valuable insight for demand forecasting and inventory management.

💡 Key Takeaways
A well-cleaned dataset can provide deep insights into customer and business behavior.

Feature engineering enhances the analytical power of raw data.

Visualizations make complex data easy to interpret and communicate.

Understanding sales patterns helps make informed strategic business decisions.

🚀 Future Work and Extensions
You can extend this notebook further by:

Building predictive models for profit, sales, or customer churn

Creating an interactive dashboard using tools like Plotly Dash or Power BI

Deploying the project using Streamlit, Flask, or FastAPI

Adding geospatial analysis with folium or geopandas

