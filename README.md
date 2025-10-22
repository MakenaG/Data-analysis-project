#  Global Jobs Data Analysis
## 📌 Overview
This project explores global job postings to uncover patterns in **categories, countries, seniority, and contract types**.  
The workflow demonstrates a full analytical pipeline — from **data cleaning in SQL Server (SSMS)** to **analysis and visualization in Excel**.

## DASHBOARD APP LINK
This project highlights practical data analysis, cleaning, and storytelling skills that mirror real-world business intelligence workflows. below is an app to upload the cleaned dataset to generate the dashboard: [https://899c75e2-39e8-4a1c-ab04-4b0e80519cea-00-2yhvvp9kpczv2.worf.replit.dev/]

---

## 🧭 Workflow Summary
**1. Data Source:** Raw job postings dataset collected from Kaggle(path = kagglehub.dataset_download[https://www.kaggle.com/datasets/techsalerator/job-posting-data-in-kenya].  
**2. Cleaning:** Performed in **SQL Server Management Studio (SSMS)** using SQL queries to remove invalid entries and handle missing data.  
**3. Export:** Cleaned data exported to **Excel** as `Jobs_Cleaned.xlsx` for analysis.  
**4. Analysis:** Conducted using **PivotTables** and **interactive slicers**.  
**5. Visualization:** Designed a polished **Excel dashboard** summarizing key trends.

---

## 🧹 Data Cleaning (SQL Server)
**Main cleaning steps performed in SSMS:**
- Removed blank rows and incomplete records.
- Standardized text formatting for key columns (`Category`, `Country`, `ContractTypes`).
- Dropped salary columns with too many missing or inconsistent entries.
- Verified column data types (ensuring text, dates, and numbers were properly typed).
- Exported the final cleaned dataset to Excel using:
  ```sql
  SELECT * 
  INTO JobsCleaned

  ## 📈 Dashboard KPIs

The Excel dashboard highlights the following key performance indicators (KPIs):

| KPI | Description | Insight |
|------|--------------|----------|
| **Total Job Openings** | Total count of job listings analyzed | Overall hiring activity |
| **Active Categories** | Number of distinct job categories | Market diversity by role type |
| **Active Countries** | Number of countries represented | Geographic reach of listings |
| **Top Hiring Category** | Category with the highest job count | Field with the strongest demand |
| **Top Hiring Country/City** | Country or city posting the most jobs | Key hiring hub |
| **Most Common Contract Type** | Contract type most frequently listed | Employment structure preference |
| **Dominant Seniority Level** | Seniority level with the most openings | Talent focus (Entry, Mid, Senior) |
| **Top Job Source** | WebsiteDomain with most postings | Most active job platform |
| **Job Language Split (%)** | % distribution of job postings by language | Linguistic inclusivity of job markets |

---

### 🩵 Dashboard Features
- Interactive slicers for **Country**, **ContractTypes**, and **JobLanguage**
- Dynamic pivot-based visuals (bar, column, and map charts)
- KPI summary tiles with real-time updates
- Clean color palette and layout for presentation or sharing
