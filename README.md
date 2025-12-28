 
# Retail Sales Exploratory Data Analysis (EDA)

This project performs an automated Exploratory Data Analysis (EDA) on retail sales data to uncover insights into sales trends, regional performance, product and customer behavior, payment methods, and sales representative effectiveness.

## Project Overview

The notebook `Retail_Sales_EDA.ipynb` processes retail sales data, generates various visualizations, and provides key business insights and recommendations. It leverages Python libraries such as `pandas` for data manipulation and `plotly` for interactive visualizations.

## Features

-   **Data Loading and Preprocessing**: Loads retail sales data from an Excel file, converts date columns, extracts date features (Year, Month, Day, Weekday), and calculates `Sales_Amount` and `Revenue`.
-   **Comprehensive Dataset Overview**: Provides a summary of key metrics like total orders, customers, products, regions, date range, total revenue, and average order value.
-   **Sales Trend Analysis**: Visualizes monthly revenue trends and order counts to identify patterns over time.
-   **Regional Analysis**: Breaks down revenue, orders, and unique customers by region.
-   **Product and Category Analysis**: Identifies top-performing products and categories based on revenue and order counts.
-   **Customer Analysis**: Analyzes customer behavior, including top customers by revenue and orders, and provides customer segmentation insights.
-   **Payment Method Analysis**: Examines the distribution of revenue, orders, and customers across different payment methods.
-   **Sales Representative Performance**: Evaluates sales representatives based on revenue, orders, customers, and quantity sold.
-   **Discount Analysis**: Investigates the impact of discount rates on average revenue, order count, and average quantity sold.
-   **Business Insights and Recommendations**: Generates actionable insights and strategic recommendations based on the EDA findings.
-   **HTML Report Export**: Exports the entire EDA report, including all visualizations, into a single, interactive HTML file.

## Data

The project expects a dataset named `Retail_Sales_Data.xlsx` in the `/content/` directory. The dataset should contain columns such as 'Date', 'Quantity', 'Unit Price', 'Discount', 'Order ID', 'Customer Name', 'Region', 'Product', 'Category', 'Payment Method', and 'Sales Rep'.

## Setup and Usage

To run this notebook and generate the EDA report, follow these steps:

1.  **Clone the repository (if applicable) or download the notebook.**
2.  **Upload `Retail_Sales_Data.xlsx` to your Google Colab environment** (or ensure it's in the specified path `/content/`).
3.  **Install necessary libraries**: The first code cell automatically installs `plotly`, `pandas`, `numpy`, `openpyxl`, and `kaleido`.
4.  **Run all cells in the notebook.**
    -   The preprocessing step (`df_processed = preprocess_retail_data(df)`) will clean and enrich the raw data.
    -   The `generate_retail_sales_report(df_processed)` function will execute all EDA functions and store the generated Plotly figures.
    -   The notebook will then display all figures sequentially.
    -   Finally, `generate_business_insights(df_processed)` will print key textual insights and recommendations.
    -   `export_report_to_html(retail_report)` will save the interactive report to `retail_sales_eda_report.html`.

## Output

Upon successful execution, the notebook will:

-   Display a series of interactive Plotly visualizations covering various aspects of the retail sales data.
-   Print a section of 
