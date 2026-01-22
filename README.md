# Customer Shopping Trends Analysis

This project executes a full-cycle data engineering and analytics workflow to transform raw consumer data into actionable business intelligence.

#### # Project Overview
The analysis tracks the complete data lifecycle, from initial ingestion and cleaning to relational modeling and executive reporting.
1. Data Cleaning: Performed exploratory data analysis (EDA) to identify null values and implemented feature engineering using Python.
2. Database Management: Integrated cleaned datasets into a PostgreSQL environment for persistent storage and high-performance querying.
3. Data Analysis: Leveraged advanced SQL scripts to extract specific business metrics and solve complex analytical questions.
4. Data Visualization: Developed an interactive dashboard to communicate key performance indicators (KPIs) through visual storytelling.

#### # Tech Stack
1. Language: Python using the Pandas library for data manipulation and SQLAlchemy for automated database connectivity.
2. Database: PostgreSQL for relational data management and advanced querying.
3. Visualization: Power BI for creating multi-dimensional interactive reporting dashboards.
4. Tools: Jupyter Notebook for iterative development and VS Code for script and environment management.

#### # File Structure
1. **customer_analysis.ipynb**: Contains the end-to-end ETL pipeline including data cleaning, imputation, and PostgreSQL ingestion logic.
2. **customer_data_analysis.sql**: SQL script containing 10+ complex queries designed for business trend analysis and performance ranking.
3. **Customer_analysis_dashboard.pbix**: The visual dashboard file designed for executive-level interactive reporting.
4. **.gitignore**: Security configuration to prevent tracking of sensitive .env files and large raw datasets.

#### # Key Data Engineering Steps (Python)
1. Missing Value Imputation: Addressed null values in the `review_rating` column by applying category-specific medians to preserve accuracy.
2. Feature Engineering: 
    * Created a binned `age_group` attribute using quartile-based segments for demographic targeting.
    * Transformed qualitative frequency strings into a numerical `purchase_frequency_days` format for quantitative analysis.
3. Optimization: Standardized all column headers to snake_case and removed redundant features like `promo_code_used` for a clean relational schema.
4. Automated ETL: Programmatically migrated the final cleaned DataFrame to the PostgreSQL database using an engine-based SQLAlchemy pipeline.

#### # SQL Insights (PostgreSQL)
1. Revenue by Gender: Analyzed total and average purchase amounts to identify spending variances between demographic groups.
2. Customer Segmentation: Used Common Table Expressions (CTEs) to classify buyers as "New," "Returning," or "Loyal" based on purchase counts.
3. Product Performance: Employed Window Functions (`ROW_NUMBER`) to rank and identify the top 3 products by popularity within each category.
4. Promotion Impact: Calculated the "Discount Adoption Rate" per product using conditional aggregations to measure promotional effectiveness.

#### # Dashboard Highlights
1. Revenue Attribution: Comprehensive visual breakdowns of revenue streams across gender, age groups, and various geographical locations.
2. Operational Metrics: Real-time tracking of average review ratings and total transaction volumes.
3. Subscription Impact: Comparative analysis of spending behaviors and total revenue contribution between subscribers and non-subscribers.

<p align="center">
  <img width="1122" height="593" alt="Customer Shopping Dashboard" src="https://github.com/user-attachments/assets/b41768ea-7435-444e-9276-2e3803bd4496" />
</p>