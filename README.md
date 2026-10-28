# Retail Sales Dashboard — README

## Project overview

This Excel project analyzes online retail sales using data from the UCI Machine Learning Repository's **Online Retail** dataset.

- Source: [UCI Online Retail](https://doi.org/10.24432/C5BW33)
- The workbook includes 6,000 regularly spaced source rows and a 500-row cleaned sample selected across the full date range, December 2010 to December 2011.
- The original UCI dataset contains 541,909 records. This workbook uses a smaller sample to keep the practical project responsive.

## Workbook sheets

- **Dashboard** — filtered KPIs and charts for revenue by country, monthly revenue, and leading products.
- **Analysis** — formula-driven summaries for countries, months, products, and customers, plus VLOOKUP, INDEX-MATCH, and nested IF examples.
- **Clean Data** — cleaned sales lines with calculated revenue, revenue band, month, and year. The data is stored in the `CleanTransactions` Excel Table.
- **Raw Data** — the sampled source rows before cleaning.
- **Project Guide** — dataset provenance, cleaning rules, exam checklist, and Excel instructions.

## Cleaning rules

The cleaned sample excludes duplicate rows, cancelled invoices, nonpositive quantity or unit price, missing required product/customer fields, and malformed dates. Revenue is calculated as quantity multiplied by unit price. Currency is British pounds (GBP), matching the source dataset.

## Using the dashboard

1. Open `Mahir_ExcelDashboard.xlsx` in Microsoft Excel.
2. Use the **Country filter** and **Month filter** dropdowns at the top of the Dashboard. Choose **All** to clear a filter.
3. The KPI cards update with the selected filters. Analysis tables and charts summarize the complete cleaned sample.
4. Change the input country in `Analysis!B23` to try the VLOOKUP example.

## Adding native PivotTables, slicers, and a timeline in Excel

The workbook contains formula-driven summary tables and dropdown filters. To demonstrate the native Excel features in the exam rubric:

1. Go to **Clean Data** and select a cell in the `CleanTransactions` table.
2. Choose **Insert → PivotTable** and place the PivotTable on a new sheet or on **Pivot Tables**.
3. Create summaries such as **Country** in Rows and **Revenue** in Values. Repeat for **Month** and **Description/Product**.
4. Select a PivotTable and choose **PivotTable Analyze → Insert Slicer**. Add **Country** and/or **Description**.
5. Choose **PivotTable Analyze → Insert Timeline**, select **InvoiceDate**, then use **Report Connections** to connect the controls to all relevant PivotTables.
6. Add PivotCharts from the PivotTables if your instructor requires pivot-linked charts.

The project screenshots show a task time limit of 180 minutes, while listed estimates total 210 minutes. The listed weights total 70% because the Pivot Tables task is shown as −15%. Confirm those values with your instructor.

## Refreshing

The dashboard uses formulas and an Excel Table. If you replace the Clean Data rows, preserve the column headers and table structure. Review the cleaning rules before adding new data. Use **Formulas → Calculate Now** if Excel does not refresh the dashboard automatically.
