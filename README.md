# Avenue Mart Sales & Performance Analysis

An end-to-end Microsoft Excel project focused on preparing retail sales data, analysing business performance, and presenting findings through an interactive dashboard.

## Project Overview

Avenue Mart is a fictional retail business used for this portfolio project. The workbook takes raw sales order data through a data-cleaning process and turns it into PivotTable summaries and an interactive dashboard.

The project demonstrates how Excel can be used not only to organize and analyse sales data, but also to identify business issues and communicate possible actions to decision-makers.

> **Dataset disclosure:** This project uses synthetic data created for portfolio practice. Avenue Mart is fictional, and the customer details do not represent real people or transactions.

## Data Preparation and Cleaning

The workbook follows a simple Bronze-to-Silver data preparation approach.

- **Bronze layer:** Retains the original, uncleaned sales dataset.
- **Silver layer:** Contains the cleaned and prepared data used for analysis.

The following transformations were documented in Power Query:

| Field | Cleaning / transformation performed |
|---|---|
| Order ID | Re-created the order ID sequence |
| Order Date | Filled missing dates using the preceding date value and separated date and time into different columns |
| Customer Name | Standardized capitalization and trimmed extra spaces |
| Customer Email | Replaced the `example.com` domain with `gmail.com` and removed null email records |
| City and State | Standardized capitalization and trimmed extra spaces |
| Region | Standardized capitalization, trimmed spaces, and corrected some unknown values |
| Product Name and Category | Standardized capitalization and trimmed extra spaces |
| Supplier | Standardized capitalization and trimmed extra spaces |
| Quantity | Replaced null quantities with a default value of 1 |
| Gross Sales | Recalculated the column |
| Net Sales | Recalculated the column |
| Profit | Recalculated the column |
| Sales Channel and Payment Method | Standardized capitalization and trimmed extra spaces |
| Order Status | Standardized capitalization and trimmed extra spaces |
| Ship Date | Removed missing shipping-date records |
| Sales Representative | Standardized capitalization and trimmed extra spaces |

The Bronze sheet is retained separately so the original source data remains available for comparison.

## Tools and Excel Features

- **Microsoft Excel**
- **Power Query** for data cleaning and transformation
- **PivotTables** for summarizing sales and performance metrics
- **PivotCharts / Excel charts** for visual analysis
- **Slicers** for interactive filtering
- **KPI calculations** for revenue, cost, profit, and profit margin

## Dashboard

The dashboard brings the analysis together in one interactive view.

### Key Performance Indicators

- Total Orders
- Net Revenue
- Gross Revenue
- Cost of Goods
- Net Profit
- Net Profit Margin

### Visual Analysis

- Monthly Sales Trend
- Order Status Distribution
- Sales Channel Distribution
- Top 5 Categories by Revenue
- Monthly Revenue vs. Profit

### Interactive Filters

Users can filter the dashboard using:

- Year
- Region
- Payment Method

The slicers make it possible to explore how sales performance changes across different periods, regions, and payment methods.

## Understanding Core Business Problem

A retail business needs a clear view of its sales performance and the factors that may be affecting orders and profitability. Raw transaction data alone does not make it easy to identify patterns, compare performance, or spot operational concerns.

This project uses Excel to explore sales trends, order outcomes, product-category performance, sales channels, revenue, and profit. The analysis focuses on two business areas:

### 1. Cancelled Orders

The analysis identifies an order cancellation rate of **9.2%**.

This raises questions about the customer experience and order fulfilment process. The areas suggested for further investigation are:

- **Shipping costs:** Review whether shipping charges may be contributing to cancellations.
- **Delivery timelines:** Investigate whether delivery or shipping time is affecting customers' decisions to cancel.
- **Product quality:** Review product quality and checks before dispatch to help reduce cancellations caused by incorrect or unsatisfactory products.

The workbook notes a **1.5%–4% comparison range** for cancellation rates. This is treated as a project reference point; it should be supported by a reliable industry or company benchmark before being presented as an established industry standard.

### 2. Revenue and Profit Margin

The analysis reports that profit margin increased from **26.61% in the previous year to 27.42% in the current year**.

At the same time, the number of orders decreased by **8**. This suggests that improved margin did not coincide with order growth.

Possible actions to investigate include:

- Reviewing marketing activities and promotions to attract new customers.
- Studying changes in order volume alongside revenue and profit.
- Identifying the products, categories, regions, and sales channels contributing to revenue and profitability.

These observations are intended to guide further business investigation; they do not establish the causes of cancellations or the change in order volume.

## Workbook Structure

| Worksheet | Description |
|---|---|
| `README` | Dataset notes, documented cleaning steps, and business problem observations |
| `Raw_Data_Bronze` | Original raw sales dataset |
| `Raw_Data_Silver` | Cleaned dataset prepared for analysis |
| `Pivot_Table` | PivotTable summaries and supporting calculations |
| `Dashboard` | Interactive sales and performance dashboard |

## How to Explore the Project

1. Download the Excel workbook from this repository.
2. Open it in the desktop version of Microsoft Excel.
3. Review `Raw_Data_Bronze` to understand the original source data.
4. Review `Raw_Data_Silver` to see the cleaned dataset.
5. Open `Pivot_Table` to inspect the supporting summaries.
6. Open `Dashboard` and use the slicers to explore the results.

If you make changes to the source data or Power Query steps, refresh the queries and PivotTables to update the analysis. Some Excel features, including slicers and PivotTables, are best explored in desktop Excel.

## Repository Contents

```text
avenue-mart-sales-performance/
├── README.md
├── Avenue_Mart_Sales_Performance.xlsx
└── screenshots/
    ├── avenue-mart-dashboard.png
    ├── avenue-mart-data-cleaning.png
    └── avenue-mart-pivot-analysis.png
```

## Project Takeaways

Through this project, I practised:

- Cleaning and preparing raw sales data using Power Query.
- Applying a Bronze-to-Silver data preparation workflow.
- Building PivotTables to analyse sales and operational performance.
- Creating an interactive Excel dashboard with slicers.
- Interpreting revenue, profit margin, order trends, and cancellation patterns.
- Translating analysis into business questions and possible recommendations.

## Author

**Gaurav Khanna**

- [LinkedIn](https://www.linkedin.com/in/gauravkhanna03)
- [Portfolio](https://gouravkhanna03.github.io/portfolio/)
- [GitHub](https://github.com/gouravkhanna03)
