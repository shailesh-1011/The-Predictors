Revenue Data Analysis

Overview :

This project aims to analyze calendar year revenue data to identify trends, seasonal patterns, and key contributing factors. By combining Python for data cleaning, SQL for structured storage, and Power BI for visualization, this end-to-end workflow delivers actionable insights.

Key Objectives:

Prepare the raw revenue data for analysis by handling missing values, standardizing formats, and deriving useful features.
Store the cleaned data in an SQL database with a well-designed schema for efficient querying and analysis.
Visualize revenue trends through an interactive Power BI dashboard that provides insights into yearly, monthly, and category-specific performance.
Enable real-time updates for the Power BI dashboard to reflect new data seamlessly.
Project Workflow

Step 1: Data Cleaning (Python)
The raw dataset (calendar_year_revenue.csv) is processed to ensure data quality and usability. This involves:
Filling or handling missing values appropriately.
Standardizing date formats and ensuring revenue data is numerical.
Adding additional columns, such as:
year and month (derived from dates).
revenue_category, which classifies revenue into categories like Low, Medium, and High based on thresholds.
Saving the cleaned dataset as a CSV file for further use.

Step 2: SQL Database Integration
The cleaned data is stored in an SQL database for structured analysis.
A database schema is designed with the following tables:
revenue_data: Stores the main dataset with columns like date, revenue, year, month, and revenue category.
date_details (optional): Provides additional context, such as fiscal quarters or holidays.
Python is used to load the data into the database using libraries like SQLAlchemy.

Step 3: Power BI Dashboard
The Power BI dashboard connects to the SQL database and provides interactive visualizations:
Line Chart: Revenue trends over time (e.g., yearly or monthly).
Bar Chart: Comparison of revenue categories across different months or years.
KPI Cards: Metrics like total revenue, year-over-year (YoY) growth, and top-performing months.
Filters and Slicers: Allow users to explore data by date ranges, revenue thresholds, and categories.

Step 4: Real-Time Updates
To ensure the dashboard reflects the latest data:
The SQL database is periodically updated with new records using an automated Python script.
Power BI is configured to refresh data on a scheduled basis, ensuring it stays in sync with the database.
How to Set Up the Project

Prerequisites:
Python 3.x installed on your system.
A SQL database (e.g., SQLite, PostgreSQL, or MySQL).
Power BI Desktop installed for creating and viewing the dashboard.
Basic knowledge of Python, SQL, and Power BI.
