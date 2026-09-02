# Analysis Notes — Sales Data (2022–2026)

## PivotTable Findings

### Revenue by Region
- West: $483,569.10 (highest)
- North: $472,519.81
- East: $456,737.45
- South: $424,294.87 (lowest)

The gap between the highest and lowest region is roughly 12%.

### Revenue by Product Category
- Electronics (highest)
- Clothing
- Home
- Beauty (lowest)

### Revenue by Year (2022–2026)
- Trend is mixed — up, then down, then up again — not a steady linear growth pattern
- 2026 confirmed to be a full year of data (through December), so the upward end-point is not an artifact of a partial year
- Nested Month-within-Year grouping available in the Pivot for further seasonality investigation if needed

## KPI Summary
- Total Revenue: $1,837,121.23
- Total Orders: 1,826
- Average Order Value: $1,006.09
- Total Quantity Sold: 7,343
- Average Discount: 18%

## Dashboard
- Built single-page dashboard with 5 KPI cards + 3 charts (revenue by region, revenue by category, revenue by year trend)
- Chart types: bar charts for region/category comparisons, line chart for year trend
- Screenshot: screenshots/dashboard-overview.png

## Interactivity
- Added `region`, `product_category`, and `year` slicers, connected to all 3 PivotCharts via Report Connections
- Verified: selecting a value (e.g., "West") correctly filters all 3 charts simultaneously
- Slicers positioned on the left side of the Dashboard sheet, resized to show all values without scrolling

## Scope Note
Analysis limited to 2022–2026, despite the raw dataset containing order dates through 2035, to reflect a realistic recent business time frame.
