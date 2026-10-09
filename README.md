# E-Commerce Sales Analysis \| Excel Project

## Project Overview

This project analyzes an e-commerce sales dataset using Microsoft Excel.
It explores sales performance, product categories, customer
demographics, payment methods, store types, regional performance, and
inventory levels. The goal is to turn raw sales data into useful
business insights and practical recommendations.

## Business Objectives

-   Understand overall sales performance and sales trends.
-   Compare sales across product categories, regions, store types, and
    payment methods.
-   Explore customer demographics and purchasing patterns.
-   Identify products that may need inventory review by comparing stock
    with historical sales.
-   Develop recommendations to support inventory planning, marketing,
    and business decisions.

## Dataset Overview

The workbook contains **2,000 sales records** covering **14 October 2023
to 13 October 2025**, along with customer, product, and store dimension
tables.

Key fields in the sales data include:

-   `Order_Date`
-   `Customer_ID`
-   `Product_ID`
-   `Prod_Category` and `Prod_Sub_Category`
-   `Store_ID` and `Store_Type`
-   `Quantity`
-   `Unit_Price`
-   `Discount`
-   `Payment_Type`
-   `Total_Amount`

The workbook also contains customer, product, and store dimension tables
that provide additional context for the sales records.

## Workbook Structure

  -----------------------------------------------------------------------
  Worksheet                           Purpose
  ----------------------------------- -----------------------------------
  `Sales_Data`                        Main sales dataset used for
                                      analysis.

  `Dashboard`                         Visual summary of selected sales
                                      metrics and charts.

  `Descriptive_Statistics`            Summary statistics for sales
                                      amount, discount, unit price, and
                                      quantity.

  `ProductvsStockvsAmt`               Product-level comparison of stock
                                      and total sales.

  `YearvsAmt`                         Total sales grouped by year.

  `CategoryvsQtyvsAmt`                Quantity sold and total sales by
                                      product category.

  `PaymentvsSales`                    Sales comparison by payment method.

  `AgevsSales`                        Customer demographic analysis.

  `RegionvsSales`                     Sales comparison by region.

  `Customer_Dim`                      Customer attributes such as age,
                                      age group, gender, location, and
                                      loyalty level.

  `Product_Dim`                       Product attributes including
                                      category, subcategory, cost, stock,
                                      and historical sales.

  `Store_Dim`                         Store attributes including region,
                                      city, and store type.

  `Sales_Fact`                        Transaction-level fact table with
                                      sales IDs and measures for
                                      analysis.
  -----------------------------------------------------------------------

## Data Cleaning and Preparation

The workbook includes data-cleaning and transformation work, such as:

-   Handling missing values in selected fields.
-   Standardizing inconsistent customer and product identifiers.
-   Imputing missing product cost values using the average for the
    corresponding subcategory.
-   Imputing missing stock values and ensuring stock values are
    represented as whole units where appropriate.
-   Creating customer age groups for demographic analysis.
-   Preparing fact and dimension tables for analysis.

> Data-cleaning decisions should be documented and validated before the
> workbook is used for business-critical decisions. Imputed values are
> estimates and may affect results.

## Analysis Performed

### Descriptive Analysis

-   Summary statistics for sales amount, discount, unit price, and
    quantity.
-   Sales by year, product category, payment method, region, and store
    type.
-   Product-level comparison of stock and total sales.
-   Customer demographic exploration.

### Predictive Analysis --- Suggested Extension

The workbook can be extended with a monthly sales forecast using Excel's
`FORECAST.ETS` function. Forecasting should be based on consistently
aggregated monthly data and compared with actual results over time. The
current dataset covers roughly two years, so seasonal patterns should be
interpreted cautiously.

### Prescriptive Analysis --- Suggested Extension

Potential decision-support analyses include:

-   Ranking products for stock review using recent sales velocity and
    available stock.
-   Calculating reorder points using average demand, supplier lead time,
    and safety stock.
-   Testing targeted promotions while monitoring profit margin.
-   Investigating regional sales differences before reallocating
    marketing spend.
-   Tracking forecast accuracy and updating inventory plans as new sales
    data arrives.

These are recommendations for further analysis; they should not be
treated as completed model outputs unless the relevant calculations have
been added to the workbook.

## Key Findings

The following findings are based on the workbook's recorded sales
values:

-   **Total recorded sales:** approximately **2,174,394.70** across
    2,000 sales records.
-   **Top sales category:** Sports, with approximately **542,010.17** in
    sales.
-   **Second-highest category:** Electronics, with approximately
    **504,311.35** in sales.
-   **Top payment method by sales amount:** PayPal, with approximately
    **756,754.57**.
-   **Top store type by sales amount:** Online, with approximately
    **914,253.52**.
-   **Highest-sales region:** North, with approximately **646,100.88**.
-   **Lowest-sales region:** West, with approximately **270,676.41**.
-   **Average recorded discount:** approximately **14.80%**.
-   **Comparable-period trend:** Sales from January--September 2025 were
    approximately **2.34% higher** than January--September 2024.

These findings describe the values in this dataset. They do not by
themselves establish profitability, causation, stockout risk, or future
performance. Regional comparisons may also be affected by differences in
store coverage or operating conditions.

## Business Recommendations

1.  **Review inventory by product.** Use recent demand, current stock,
    and supplier lead times to decide which products need replenishment.
2.  **Investigate high-performing categories.** Review best-selling
    products in Sports and Electronics and check whether they also
    deliver healthy margins.
3.  **Investigate regional differences.** Review the reasons for lower
    recorded sales in West before deciding whether to change marketing
    or distribution.
4.  **Evaluate promotions by profitability.** Assess whether discounts
    improve conversion and total profit, not just revenue.
5.  **Use forecasts as planning estimates.** Compare forecast sales with
    actual sales and revise plans as new data becomes available.
6.  **Monitor business KPIs.** Track monthly sales growth, gross margin,
    inventory turnover, stockout rate, average order value, and repeat
    purchase rate where the required data is available.

## Tools and Skills

-   Microsoft Excel
-   Data cleaning and transformation
-   Excel formulas and lookup functions
-   Descriptive statistics
-   PivotTables and charts
-   Dashboard reporting
-   Business insights and recommendations
-   Introductory predictive and prescriptive analysis concepts

## How to Use This Project

1.  Download or clone this repository.
2.  Open `Ecommerce_Sales_Dataset_updated(3).xlsx` in Microsoft Excel.
3.  Start with the `Dashboard` worksheet for a high-level overview.
4.  Review the analysis worksheets for category, region, payment,
    product, and customer findings.
5.  Review the source and dimension sheets when validating a result or
    extending the analysis.

## Limitations

-   The dataset covers a limited historical period and may not represent
    future demand.
-   The dataset's final month is partial, so it should not be compared
    directly with complete months.
-   Historical sales and current stock snapshots alone are not enough to
    calculate reliable stockout probabilities.
-   Profitability analysis requires validated cost and margin
    calculations.
-   Forecasts and recommendations should be validated against new data
    before operational use.

## Project Files

-   `Ecommerce_Sales_Dataset_updated(3).xlsx` --- Excel workbook
    containing the dataset, analysis sheets, and dashboard.
-   `README.md` --- Project overview, workbook guide, findings, and
    recommendations.

## Author

**Your Name**\
*Excel Data Analysis Project*
