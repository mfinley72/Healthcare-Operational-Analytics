# Healthcare Operational & Financial Analytics Portfolio

## 📌 Project Overview
This project demonstrates an end-to-end data analytics workflow applied to a large-scale healthcare dataset containing over 45,000 patient records. The objective was to clean raw hospital operational data using Python and construct interactive, executive-ready dashboards in **both Power BI and Tableau** to analyze hospital revenues, patient demographics, and admission pipelines.

Building identical analytical interfaces across both industry-standard BI platforms proves cross-tool proficiency, demonstrating tool-agnostic architecture and data logic.

* **Interactive Tableau Dashboard:** [[👉 (https://public.tableau.com/shared/SJ2T4HWK4?:display_count=n&:origin=viz_share_link)
* **Power BI Project File (.pbix):** [👉 Available inside the /dashboards folder of this repository]

---

## 🛠️ Technical Workflow & Architecture

### 1. Data Cleaning & Engineering (Python / Pandas)
The raw dataset required normalization and structural formatting before visualization to ensure cross-platform consistency:
* **Missing Value Imputation:** Checked data distributions and stabilized numerical entry fields.
* **Text Normalization:** Standardized mixed-casing across medical diagnoses and health insurance provider names to prevent duplicate categories.
* **Demographic Binning:** Engineered a custom categorical variable `Age Group` (`0-17`, `18-34`, `35-49`, `50-64`, `65+`) using Pandas to optimize cross-tabular performance reporting.

### 2. Operational Dashboards (Power BI Desktop)
Built an operational health center snapshot focusing on high-level executive performance metrics:
* **KPI Card Elements:** Tracks Total Revenue ($1.42B), Total Patient Admissions (~55K), and Overall Average Patient Age (51.5 years).
* **Categorical Slicers:** Implemented fully responsive drop-down interactive filters enabling immediate data segmentation by specific hospitals and arrival status.
* **Cross-Filtering Matrix:** Evaluated categorical medical operational dependencies across age buckets.

### 3. Advanced Behavioral Diagnostics (Tableau Public)
Designed a deep-dive workspace leveraging Tableau's advanced data visualization engine:
* **Patient Distribution Heat Map:** Uses custom grid visual densities to expose numerical patient volumes across intersectional variables.
* **Continuous Financial Trend Line:** Generates an ongoing time-series analysis evaluating cyclic hospital spending behaviors across multi-year admission date streams.
* **Interactive Filter Actions:** Configured a global dashboard action where selecting any cell in the demographic heat map dynamically filters the continuous timeline view.

---

## 📈 Key Data Insights Discovered
* **Financial Equality Across Payers:** Total billing volumes show an almost perfectly equal split among core commercial insurance providers (Cigna, Blue Cross, Medicare, UnitedHealthcare, Aetna), indicating highly consistent cross-network hospital contract pricing tiers.
* **Demographic Revenue Spread:** The average billing cost remains consistently flat around $26k–$28k regardless of the medical condition or age group, indicating a highly uniform operational cost structure.
* **Stable Admission Flow:** Elective, Urgent, and Emergency admission modes share a uniform distribution, proving that hospital facilities maintain consistent administrative loads across all operational categories.

---

## 🚀 How to Review This Project
1. Open the `/notebooks/` directory to inspect the Python pipeline used for processing the data layers.
2. Download the `.pbix` file from the `/dashboards/` directory to view the Power BI model architecture locally.
3. Visit the Tableau Public link above to experience the responsive dashboard actions live.

