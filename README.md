Customer Shopping Trends Analysis
This project executes a full-cycle data engineering and analytics workflow to transform raw consumer data into actionable business intelligence.

Project Overview
The analysis tracks the complete data lifecycle, from initial ingestion and cleaning to relational modeling and executive reporting.

Data Cleaning: Performed exploratory data analysis (EDA) and feature engineering using Python.

Database Management: Integrated cleaned datasets into a PostgreSQL environment for persistent storage and high-performance querying.

Data Analysis: Leveraged advanced SQL to extract specific business metrics and trends.

Data Visualization: Developed an interactive dashboard to communicate key performance indicators (KPIs).

Tech Stack
Language: Python (Pandas for manipulation, SQLAlchemy for database connectivity).

Database: PostgreSQL for relational data management.

Visualization: Power BI for multi-dimensional reporting.

Tools: Jupyter Notebook for development and VS Code for script management.

File Structure
customer_analysis.ipynb: Contains the ETL pipeline including data cleaning and PostgreSQL ingestion logic.

customer_data_analysis.sql: SQL script containing 10 complex queries for business trend analysis.

Customer_analysis_dashboard.pbix: The visual dashboard file for interactive reporting.

.gitignore: Security configuration to prevent tracking of sensitive .env files and large datasets.

Key Data Engineering Steps (Python)
Missing Value Imputation: Addressed null values in Review Rating by applying category-specific medians to preserve data distribution.

Feature Engineering:

Created a binned age_group attribute (Young Adult, Adult, Middle-aged, Senior) using quartile-based segments.

Transformed qualitative frequency strings into a numerical purchase_frequency_days format for quantitative analysis.

Optimization: Standardized all column headers to snake_case to ensure seamless integration with the PostgreSQL schema.

Automated ETL: Programmatically migrated the final DataFrame to the database using an engine-based SQLAlchemy pipeline.

SQL Insights (PostgreSQL)
Revenue by Gender: Analyzed total and average purchase amounts to identify spending variances between demographic groups.

Customer Segmentation: Used Common Table Expressions (CTEs) to classify buyers as "New," "Returning," or "Loyal" based on historical purchase counts.

Product Performance: Employed Window Functions (ROW_NUMBER) to rank the top 3 products by popularity within each category.

Promotion Impact: Evaluated the adoption rate of discounts across different item categories to measure promotional effectiveness.

Dashboard Highlights
Revenue Attribution: Comprehensive visual breakdowns of revenue by gender, age group, and geographic location.

Operational Metrics: Tracking of average review ratings and total transaction volumes.

Subscription Impact: Comparative analysis of spending behaviors between subscribers and non-subscribers.