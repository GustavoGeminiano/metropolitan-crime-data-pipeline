# 🚨 Metropolitan Crime Data Pipeline & Analytical Dashboard

An end-to-end Data Engineering and Data Science project that extracts, cleans, and analyzes 8 years of public safety and crime data (2017–2024) across 9 coastal municipalities. 

This project processes over 99 raw, unorganized Excel spreadsheets into a unified analytical pipeline using **Python (Parallel Processing & Pandas)** and renders key public policy metrics in an interactive **Power BI Dashboard**.

---

## 📌 Key Business & Analytical Insights

* **Standardized Rate Normalization:** Normalized raw incident counts to *Per 100k Inhabitants* to allow fair statistical comparison across cities with vastly different population sizes (ranging from 60k to 400k+).
* **Domain Filtering & Deduplication:** Filtered out non-intentional crimes and redundant metrics (e.g., separating victim counts vs. incident occurrences) to eliminate statistical noise.
* **Geographical & Temporal Trends:** Identified that property crimes (theft/robbery) account for 60%–70% of total offenses, with distinct seasonality spikes in coastal tourist hubs during high-season periods.

---

## 📊 Interactive Dashboard

You can explore the live, interactive Power BI dashboard here:
👉 **[View Live Power BI Dashboard](https://fatecspgov-my.sharepoint.com/:u:/g/personal/adriane_santos3_fatec_sp_gov_br/ER8GHVc31ypJmIvCfbV9j5UB9shFnAUlnsmWgg9w9Mt5nw?e=gOrRSs)**

---

## 🛠️ Tech Stack & Architecture

* **Data Extraction & ETL:** Python (`pandas`, `openpyxl`, `re`)
* **Performance Optimization:** Parallel Processing via `concurrent.futures.ProcessPoolExecutor` for bulk Excel file ingestion.
* **Data Visualization & Dashboards:** Power BI (DAX, Interactive Reporting)
* **Documentation & Reporting:** LaTeX

---

## 🏗️ Pipeline Overview

1. **Ingestion:** Asynchronous reading and extraction of 99+ unstructured `.xlsx` files provided by the State Public Security Department (SSP-SP).
2. **Transformation & Cleaning:**
   * String normalization and dictionary mapping for inconsistent city names (e.g., mapping `"S.VICENTE"`, `"SV"` ➔ `"SÃO VICENTE"`).
   * Schema alignment and column renaming.
3. **Aggregation:** Grouping by city, crime category, month, and year using `pandas.groupby()`.
4. **Visualization:** Export to clean CSV for Power BI ingestion, building dynamic dashboards tracking violent vs. property crime rates.

---

## 📊 Sample Visualizations & Technical Report

* The repository includes the full technical paper compiled in LaTeX detailing the complete statistical methodology and findings.

---

## 👤 Authors

* **Gustavo Nascimento Geminiano** - *Data Preparation, ETL Pipeline & Analytics*
* Adriane da Costa Santos, Arthur Galvão Torres Venceslau, Giulia Dias Granado de Marques.
* **Institution:** Fatec Baixada Santista Rubens Lara
