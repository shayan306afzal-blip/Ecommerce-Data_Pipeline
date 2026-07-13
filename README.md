# Automated E-Commerce Data Pipeline & Revenue Analytics

## 📌 Project Overview
This project builds an end-to-end local data pipeline that extracts transaction data directly from a relational **SQLite database**, executes an automated **Pandas data wrangling pipeline** to resolve real-world anomalies, and delivers a business intelligence visualization layer using **Matplotlib**.

The objective is to ingest messy transaction logs and generate a structured, executive-ready dashboard showcasing regional financial performance.

---

## 🛠️ Tech Stack & Methods
*   **Database Engine:** SQLite / `sqlite3`
*   **Data Wrangling & Pipeline:** Python 3 / Pandas / NumPy
*   **Data Visualization:** Matplotlib
*   **Environment:** Jupyter Notebook

---

## 🏗️ Data Engineering & Pipeline Architecture

### 1. Database & Schema Enforcement
*   Designed an automated table creation pipeline inside SQLite using custom relational constraints (`PRIMARY KEY`, `NOT NULL`).
*   Handled and bypassed unique constraint traps cleanly during secondary transaction batches using native backend script flow.

### 2. Automated Data Cleaning Process
The raw data contained major systematic errors. The Pandas pipeline automatically corrects the following anomalies before the reporting phase:
*   **Structural Orientation Fixes:** Resolved complex transpose and axes flip display issues (`df.T`) to restore standard relational row/column layouts.
*   **Duplicate Entry Management:** Resolved dual-value conflicts on matching user records by isolating keys and applying precise `.drop_duplicates(subset=[...], keep='first')` logic.
*   **Text & Feature Standardization:** Streamlined localized text metrics into capitalized standardized fields (`USA`, `UK`, `CANADA`).
*   **Index Calibration:** Realigned row positioning post-cleansing using sequential sorting based on `transaction_id`.

---

## 📊 Business Intelligence Insights
The finalized script processes the cleaned records, aggregates global transactions, and visualizes market share trends:

*   **Total Revenue Analysis:** Computes absolute revenue streams per active region.
*   **Visual Presentation Layer:** Displays a custom-styled bar chart featuring transparent structural spines, explicit data labels, and optimized color hierarchy for swift enterprise decision-making.

---

## 🚀 How to Run the Project
1. Clone the repository:
   ```bash
   git clone [https://github.com/shayan306afzal-blip/Ecommerce-Data_Pipeline.git]([https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/shayan306afzal-blip/Ecommerce-Data_Pipeline.git))
