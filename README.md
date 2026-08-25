# Sales Analysis Dashboard (2022–2026)

## Overview
A complete Excel-based sales analysis project, covering data cleaning, transformation,
and dashboard design using Power Query, PivotTables, and PivotCharts.

## Business Problem
This project analyzes regional and category-level sales performance from 2022–2026 to identify top and bottom performers, and support data-driven decisions on where to focus business attention.

## Tools Used
- Microsoft Excel (Tables, PivotTables, PivotCharts)
- Power Query (data cleaning, filtering, merging)
- GitHub (version control, documentation)

## Data Preparation
The original raw file was kept untouched in `data/raw/`, with all cleaning done on a separate working copy. Two broken duplicate sheets (a partial region lookup table causing missing manager data) were identified and removed from the working file. Full details: [power-query/documentation.md](power-query/documentation.md)

## Power Query Transformations
Data was loaded into Power Query, verified for quality (no missing values, no duplicate order IDs), filtered to a 2022–2026 scope, and merged with a region-manager lookup table using a Left Outer join. Full details: [power-query/documentation.md](power-query/documentation.md)

## Analysis
Three PivotTables were built to analyze revenue by region, by product category, and by year. Full details: [documentation/analysis-notes.md](documentation/analysis-notes.md)

## Dashboard
A single-page dashboard combining 5 KPI cards (Total Revenue, Total Orders, Average Order Value, Total Quantity Sold, Average Discount) with 3 charts covering regional, category, and yearly performance.
![Dashboard Screenshot](screenshots/dashboard-overview.png)

## Key Insights
- West region leads in revenue ($483,569), South trails ($424,295)
- Electronics is the top-performing category, Beauty the lowest
- Revenue shows a mixed (up-down-up) trend across 2022–2026, not a steady climb

Full details: [documentation/business-insights.md](documentation/business-insights.md)

## Dataset
- Source: Kaggle.com
- 5,000 orders originally, filtered to 1,826 orders (2022–2026 scope)
- 17 columns including region, product category, revenue, discount, payment method


## Project Structure

sales-analysis-dashboard/

├── data/raw/ → original untouched dataset

├── excel/ → working Excel file with Tables, Power Query, Pivots, Dashboard

├── power-query/ → Power Query transformation documentation

├── screenshots/ → dashboard screenshot

└── documentation/ → data dictionary, analysis notes, business insights

## Skills Demonstrated
- Excel Tables & structured references
- Power Query: cleaning, filtering, merging queries
- PivotTables & PivotCharts
- KPI calculation
- Dashboard design
- Business insight writing
- Git & GitHub version control
