# Supermarket Sales Dashboard (Excel)

An interactive Excel dashboard I made for my BCA data analysis practice. I used a real public dataset from Kaggle and followed a 7-task brief: import, cleaning, pivots, formulas, charts, dashboard and documentation.

<img width="1482" height="1410" alt="02_Dashboard" src="https://github.com/user-attachments/assets/5ebb94f6-a2d1-438d-922e-8778621cc7b9" />


## About the data

- **Dataset:** Supermarket Sales (Kaggle)
- **Size:** 1,000 bills from 3 branches (Yangon, Mandalay, Naypyitaw)
- **Period:** 1 Jan 2019 to 30 Mar 2019
- **Columns:** product line, customer type, gender, payment method, date, time, rating, total, and more

**What I wanted to find:** which product lines, cities, payment types and timings bring the most sales.

## What I found

- Total sales: **322,967** across 1,000 bills (average bill about 323).
- **Food and beverages** is the top product line (56,145, about 17.4% of sales). **Health and beauty** is the lowest (49,194).
- **Naypyitaw** has the highest sales of the three cities (110,569).
- **January** was the best month (116,292). February dropped about 16%, and March recovered about 12.6%.
- Cash, Ewallet and Credit card are close to each other in sales share (about 35%, 34% and 31%).
- The busiest hour is **19:00**.
- Average customer rating is about **6.97** out of 10.

The results are very evenly spread, so I treat these as practice insights, not business advice.

## What is inside the workbook

| Sheet | What it has |
|---|---|
| Dashboard | Main page with 3 dropdown filters (city, product line, month), 6 KPI boxes and 5 charts |
| Pivot_Analysis | 7 summary tables (product line, city x product, monthly, payment, customer x gender, time of day, hourly) |
| Formulas | VLOOKUP vs INDEX-MATCH, left lookup, two-way lookup, nested IF scorecard |
| Clean_Data | Cleaned table (tblSales) with helper formula columns |
| Raw_Data | Original CSV copy, not edited |
| Cleaning_Log | Checks I ran (duplicates, blanks, data types) |
| Chart_Data, Lists | Small tables behind the charts, dropdown lists and settings |

## Tasks and where I did them

| Task | Done in |
|---|---|
| 1. Dataset selection and import | Raw_Data |
| 2. Data cleaning and preparation | Clean_Data, Cleaning_Log |
| 3. Pivot tables | Pivot_Analysis |
| 4. Advanced formulas | Formulas, Clean_Data (columns Q to V) |
| 5. Data visualization | Dashboard charts, colour scales and data bars |
| 6. Interactive dashboard | Dashboard (dropdown filters, dynamic named ranges) |
| 7. Documentation | README sheet, Cleaning_Log |

## Skills used

SUMIFS, COUNTIFS, AVERAGEIFS, VLOOKUP, INDEX-MATCH, IF and nested IF, AND/OR, IFERROR, named ranges, data validation (dropdowns), conditional formatting, Excel Table, charts.

## Screenshots

**Dashboard with a filter applied (Yangon, Health and beauty, Feb)**

<img width="1482" height="1410" alt="03_Dashboard_Filtered_Yangon_HealthBeauty_Feb" src="https://github.com/user-attachments/assets/456585e8-a481-4d59-83a5-37fb52d7bc28" />


**Pivot analysis**

<img width="1136" height="1366" alt="04_Pivot_Analysis" src="https://github.com/user-attachments/assets/82ad7b74-cc36-4083-812a-086243e35f0c" />


**Formulas**

<img width="1448" height="1382" alt="05_Formulas" src="https://github.com/user-attachments/assets/571e31f4-2740-4396-81e5-e6e5fe74c2f6" />


**Cleaning log**

<img width="1932" height="807" alt="08_Cleaning_Log" src="https://github.com/user-attachments/assets/e7c70db2-491e-4828-b280-3dc5c94b4c80" />


## How to use

1. Download `Prince_ExcelDashboard.xlsx` and open it in Excel.
2. Go to the **Dashboard** sheet.
3. Change the yellow boxes (Branch / City, Product Line, Month). "All" means no filter.
4. Everything on the page updates. The weekly chart ignores the month filter on purpose so the full timeline always shows.

Settings such as what counts as a Large order or an Excellent rating are in the **Lists** sheet (yellow cells).

## Data notes

- Gross Income is exactly the same as the 5% tax column in every row, so it is not real profit. The margin percentage is also the same in all rows, so I did not use it.
- Currency is not given in the source, so I kept plain numbers.
- Only 3 months of data, so there is no yearly comparison.
- My pivot tables are formula based (SUMIFS and COUNTIFS), not the Excel PivotTable object. This keeps them connected to the dashboard.


```


