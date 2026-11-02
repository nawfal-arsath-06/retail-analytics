# Retail Analytics Dashboard

An end-to-end Retail Analytics Dashboard designed to analyse sales performance, profitability, product performance, customer behaviour, and regional trends using data analytics and interactive visualisations.

## Project Overview

The Retail Analytics Dashboard transforms retail transaction data into meaningful business insights. It helps understand revenue generation, profit margins, customer purchasing patterns, product performance, and regional sales distribution.

The project uses PostgreSQL for data storage and management, Python and FastAPI for backend services, React with TypeScript for the frontend application, and Microsoft Power BI for interactive business intelligence and reporting.

## Tech Stack

| Component             | Technology         |
| --------------------- | ------------------ |
| Frontend              | React + TypeScript |
| Backend               | Python + FastAPI   |
| Database              | PostgreSQL         |
| Business Intelligence | Microsoft Power BI |
| Data Processing       | Power Query        |
| Data Visualisation    | Power BI           |

## Dataset Description

The project uses four primary datasets stored in PostgreSQL.

| Dataset   | Description                                                                    |
| --------- | ------------------------------------------------------------------------------ |
| Customers | Customer details, segments, cities, states, and region identifiers             |
| Orders    | Order dates, customer IDs, product IDs, quantities, revenue, costs, and profit |
| Products  | Product names, categories, subcategories, and unit costs                       |
| Regions   | Regional identifiers, region names, and countries                              |

The datasets contain synthetic demonstration data and are intended for academic and analytical purposes.

## Repository Structure
```
Retail-Analytics-Dashboard/
│
├── 01_Raw_Data/
│   ├── customers_raw.csv
│   ├── orders_raw.csv
│   ├── products_raw.csv
│   └── regions_raw.csv
│
├── 02_Cleaned_Data/
│   └── (Cleaned datasets)
│
├── 03_PowerBI_Dashboard/
│   └── Retail_Analytics.pbix
│
├── backend/
│   └── FastAPI backend files
│
├── frontend/
│   └── React application files
│
└── README.md
```

## Dashboard Features

### 1. Sales Overview

- Total Revenue
- Total Profit
- Total Orders
- Total Customers
- Total Units Sold
- Monthly Revenue Trends
- Revenue by Product Category
- Profit by Region
- Profit Distribution by Category

### 2. Product Analysis

- Top-performing products
- Revenue by product category
- Units sold by category
- Product-wise revenue and profitability analysis

### 3. Customer & Regional Analysis

- Customer segmentation
- Regional sales performance
- Customer purchasing patterns
- Regional revenue and profitability comparisons

## Key Performance Indicators (KPIs)

The dashboard uses the following primary metrics:

- **Total Revenue:** Overall sales generated.
- **Total Profit:** Profit earned from retail transactions.
- **Total Orders:** Distinct number of orders.
- **Total Customers:** Distinct number of customers.
- **Total Units Sold:** Total quantity of products sold.

## Data Preparation

The data preparation workflow includes:

1. Extracting datasets from PostgreSQL.
2. Exporting original datasets into CSV format.
3. Inspecting and validating data using Power Query.
4. Handling missing values and inconsistencies where necessary.
5. Standardising data types and column formats.
6. Establishing relationships between the datasets.
7. Creating calculated measures using DAX.

## Database Relationships

The Power BI data model connects the following tables:

- Customers → Orders
- Products → Orders
- Regions → Orders

These relationships enable cross-table analysis and interactive filtering.

## How to Run

### Prerequisites

- Python
- Node.js and npm
- PostgreSQL
- Microsoft Power BI Desktop

### Power BI Dashboard

1. Clone this repository.
2. Navigate to `03_PowerBI_Dashboard`.
3. Open `Retail_Analytics.pbix` using Power BI Desktop.
4. Configure the PostgreSQL connection if required.
5. Refresh the dataset to view the latest available data.

## Project Objectives

- Analyse retail sales and profitability.
- Identify top-performing products and categories.
- Understand customer purchasing behaviour.
- Evaluate regional business performance.
- Build interactive dashboards for data-driven decision-making.

## Data Disclaimer

The datasets used in this project are synthetic demonstration datasets. They do not represent actual customer transactions or real-world retail business statistics.

## Author

**Naawfal Arsath**

BE Computer Science and Engineering

KCG College of Technology

---

*Retail Analytics Dashboard — Turning Retail Data into Business Insights.*
