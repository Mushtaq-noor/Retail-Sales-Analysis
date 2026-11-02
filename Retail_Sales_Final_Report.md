# Retail Sales Analysis Final Report

**Prepared by:** Mushtaq Noor  
**Period analysed:** 2015–2018  
**Tools:** Python, SQLite SQL, and Microsoft Power BI

## Objective and scope

This project examined US retail sales to identify patterns across time, products, regions, and customer segments. Technology generated the highest category sales, West led regional sales, and Consumer contributed just over half of recorded sales. These findings support further investigation of product availability, regional performance, and customer retention.

The supplied dataset contained 9,800 sales line items and 18 original columns. Each row represents a product line within an order, rather than a separate order.

## Data preparation and analysis

Python and Pandas were used to trim text, convert dates using day/month/year source formatting, validate sales, and check duplicate records. Postal codes were treated as text to preserve leading zeros. Eleven missing postal codes were retained without guessing replacements. No fully duplicated rows were identified.

Year, month, and days from order to shipment were derived for analysis. EDA explored annual and monthly sales, product categories, regions, customer segments, leading customers, and shipping modes. SQLite queries used aggregations, distinct counts, CTEs, and LAG to analyse performance and compare results with Python.

Power BI presented four KPI cards, a monthly trend, category and regional comparisons, customer segment shares, and the top five customers. A year slicer enabled interactive analysis; all-period results below cover 2015–2018.

## Key results

| Metric | Result |
|---|---:|
| Total recorded sales | 2,261,536.78 |
| Distinct orders | 4,922 |
| Distinct customers | 793 |
| Average order value | 459.48 |

Average order value is total sales divided by distinct orders. Currency is not explicitly specified in the supplied file.

## Findings and recommendations

1. **Technology led category sales at approximately 0.83 million.** Review its leading products and stock availability, and obtain margin data before increasing promotional spending.
2. **West led regional sales at approximately 0.71 million.** Investigate its product mix and customer purchasing patterns, then test whether successful practices transfer to other regions.
3. **South had the lowest regional sales at approximately 0.39 million.** Compare customer counts, order frequency, and average order value before selecting targeted sales initiatives.
4. **Consumer contributed 50.76% of sales**, compared with Corporate at 30.44% and Home Office at 18.79%. Prioritise consumer service while testing segment-specific offers for the other groups.
5. **Sean Miller ranked first by total customer sales over the full period.** Review recent activity and purchasing needs before planning retention outreach or account support.

## Limitations and conclusion

The dataset contains no profit, cost, quantity, discount, promised shipment date, or customer delivery date. Sales rankings do not establish profitability, and time to shipment does not measure delivery time or lateness. Findings describe the supplied records; dataset completeness and causes of performance differences are not established.

The project produced a consistent sales overview through Python, SQL, and Power BI. The next business step is to investigate the drivers behind the strongest and weakest groups and evaluate proposed actions using additional cost, inventory, and customer activity data.

*Source: supplied train.csv and the completed Power BI dashboard. Category and regional figures above are rounded dashboard values.*
