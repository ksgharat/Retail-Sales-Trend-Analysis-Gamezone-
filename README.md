# GameZone E-Commerce Data Analysis

## Overview
This repository contains a comprehensive data analysis of GameZone's e-commerce sales, executed entirely using Advanced Excel. The project demonstrates an end-to-end analytical workflow—from raw data ingestion and structural cleaning to pivot-based aggregation and strategic business reporting—contained within the `gamezone-orders-analysis.xlsx` file.

## Dataset Highlights
Based on the cleaned order dataset spanning 2019–2022, the analysis encompasses:
- **Total Volume:** 21,859 processed and cleaned orders.
- **Revenue Metrics:** An average order value (USD Price) of $281.41, with individual purchases ranging up to $3,146.88.
- **Top Performing Products:** 
  - Nintendo Switch (10,386 units)
  - 27in 4K gaming monitor (4,723 units)
  - JBL Quantum 100 Gaming Headset (4,296 units)

## Methodology & Frameworks
This project strictly leverages Advanced Excel techniques, avoiding external coding languages, to showcase native spreadsheet capabilities.

### 1. Data Cleaning & Standardization
- **Cross-Referencing:** Utilized `VLOOKUP`/`XLOOKUP` functions to map raw country codes to standardized global regions (e.g., matching "DE" to "EMEA").
- **String Manipulation:** Standardized inconsistent product naming conventions (e.g., consolidating variations of "27in 4K gaming monitor").
- **Date Formatting:** Corrected misaligned and inconsistent timestamps (`PURCHASE_TS`) into a uniform `PURCHASE_TS_Cleaned` date structure, extracting specific Month and Year columns for time-series analysis.

### 2. Quality Control (Issues Log)
An embedded **Issues Log** was utilized to track data integrity during the cleaning phase. This includes:
- Documenting the error type (e.g., missing dates, spelling inconsistencies).
- Calculating the error magnitude as a percentage of total rows.
- Logging the chosen resolution (whether the data was corrected via functions or left as-is due to low magnitude).

### 3. Analysis & Aggregation
- Extensive use of **Pivot Tables** to aggregate total revenue, calculate order frequencies, and evaluate product performance across different marketing channels and regions.
- Calculated custom metrics, such as `Time_to_Ship`, to evaluate operational efficiency between purchase and dispatch dates.

### 4. Strategic Reporting (SCAN Framework)
Business insights were developed using the **SCAN Framework**, documented in the `Insights Log`:
- **S**takeholder Goals: Identifying the core business question (e.g., 2019-2022 revenue trends).
- **C**olumns and Coverage: Mapping the specific data points required (USD Price, Purchase Item, Date).
- **A**ggregates and Anomalies: Identifying maximums, minimums, and outliers across the product lifecycle.
- **N**arrative and Next Steps: Translating numerical trends into actionable recommendations for product, marketing, and finance managers.

## File Structure
The `gamezone-orders-analysis.xlsx` workbook is organized into the following distinct sheets for transparency and reproducibility:
- `orders_uncleaned` & `region_uncleaned`: The raw, initial datasets.
- ` orders_cleaned` & `region_cleaned`: The transformed data ready for analysis.
- `Issues Log`: Documentation of data quality fixes.
- `Pivot_Table` / `Pivot_Table1`: Analytical aggregation models.
- `Insights Log`: Strategic business findings utilizing the SCAN framework.

## Conclusion
This portfolio project highlights how complex data transformations, rigorous quality tracking, and structured business reporting can be achieved efficiently using native Advanced Excel tools.
