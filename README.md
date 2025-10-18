# SOPS Workforce Analytics Project

## Description

This project analyses **Victorian Public Sector workforce data** by integrating the **SOPS 2020 Staff Opinion Survey** with the **SOPS 2024 Remuneration dataset**.  
The objective is to generate actionable insights into workforce engagement, remuneration trends, demographic structure, and equity outcomes across different departments, classifications, and occupations.

**Data Source:** Victorian Public Sector Commission (VPSC)

---

## Objectives

The main goals of this project are to:

- **Assess Workforce Engagement**  
  Evaluate employee satisfaction, leadership support, and workplace culture using SOPS 2020 survey responses.

- **Analyse Remuneration Patterns**  
  Examine salary distribution across VPS grades, occupations, and sectors from the 2024 dataset.

- **Identify Equity and Gender Pay Trends**  
  Investigate demographic factors influencing remuneration and engagement outcomes.

- **Compare 2020 vs 2024 Indicators**  
  Measure change in engagement, satisfaction, and pay over time.

- **Develop a Comprehensive Analytical Report**  
  Combine cleaned survey and remuneration data in Power BI to visualise workforce insights.

A personal objective of this project was to strengthen my ability to:
- Design **ETL workflows** for complex Excel-based data sources.  
- Use **Python (pandas)** for structured data preparation and validation.  
- Build dynamic, multi-page **Power BI dashboards** integrating survey and remuneration metrics.  

---

## Project Phases

### **1. Data Preparation**
- **Data Examination:** Reviewed raw Excel files (`6202005 (1).xlsx`, `SOPS-2024-Remuneration.xlsx`) and identified structure, metadata, and missing values.  
- **Data Transformation:** Standardised variable names, created ID mappings, replaced coded responses, and exported clean CSVs.  
- **Output:** `modified_files/` folder containing standardized datasets for modelling.

### **2. Data Modelling**
- **Schema Structure:** Designed star schema linking demographic, remuneration, and survey dimensions.  
- **Entity Relationships:** Established connections between `respondents`, `departments`, `occupations`, and `remuneration` tables.  
- **Data Loading:** Imported prepared CSV files into Power BI for further analysis.  

### **3. Data Analysis**
- **Python Analysis:** Conducted preliminary descriptive statistics and data validation using pandas.  
- **Key Focus Areas:**  
  - Engagement and satisfaction trends  
  - Salary distribution by grade and occupation  
  - Gender and age balance  
  - Tenure vs remuneration  
  - Leadership impact on engagement  

### **4. Report Creation**
- **Insights Presentation:** Built an interactive Power BI report visualising the 2020–2024 workforce insights.  
- **Report Pages:** Overview, Remuneration Analysis, Engagement, Demographics, and Comparative Insights.  
- **Link to Interactive Power BI Report:** [Report]  

**Disclaimer:** Salary and engagement scores may vary based on browser regional settings.  
This report was designed for the **EN-AU** region. Please adjust your Power BI regional settings if necessary.

---

## About

This project combines staff engagement and remuneration datasets to reveal **strategic workforce insights** and support **evidence-based HR decision-making** across the Victorian Public Sector.

---

## Topics
data-preparation · data-modelling · workforce-analytics · remuneration-analysis · powerbi-report · python-pandas

---

## Resources
- **Raw Data:** VPSC SOPS 2020 Survey, SOPS 2024 Remuneration Report  
- **Tools Used:** Python (pandas, openpyxl), Power BI, Excel  
- **Output Files:**  
  - `/1. Data Preparation/` – cleaning and transformation scripts  
  - `/2. Data Modelling/` – schema design and relationships  
  - `/3. Data Analysis/` – validation and statistical summaries  
  - `/4. Report Creation/` – Power BI report and presentation  

---

## Repository Structure
