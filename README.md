# 📈 Data Salary Dashboard (Microsoft Excel)

A dynamic and interactive dashboard built in **Microsoft Excel** to analyze and visualize global salary trends across various data science, engineering, and tech roles.

---

## 📋 Table of Contents
1.  [Project Overview](#1-project-overview)
2.  [Project Goal](#2-project-goal)
3.  [Key Features and Metrics](#3-key-features-and-metrics)
4.  [Data Source and Preparation](#4-data-source-and-preparation)
5.  [Technology and Tools](#5-technology-and-tools)
6.  [Snapshots](#6-snapshots)
7.  [How to Use the Dashboard](#7-how-to-use-the-dashboard)
8.  [File Structure](#8-file-structure)


---

## 1. Project Overview

This project delivers a robust **Salary Dashboard** designed to provide comprehensive insights into the compensation landscape for technical professionals, including **Data Scientists, Data Engineers, and Data Analysts**. Leveraging the powerful data processing and visualization capabilities of Microsoft Excel, the dashboard allows users to dynamically filter salary data based on job role, geographical location, and employment type.

The centerpiece of this project is the **Data Science Salary Calculator**, which provides real-time median salary estimations based on user-selected criteria.

---

## 2. Project Goal

The primary objectives of this dashboard are:

* **Transparency:** To provide a clear, easy-to-digest view of competitive salaries for various tech roles globally.
* **Actionable Insights:** To assist professionals in salary negotiations, career planning, and understanding market value.
* **Interactive Analysis:** To demonstrate proficiency in building complex, data-driven solutions using standard spreadsheet software (Excel).

---

## 3. Key Features and Metrics

The dashboard provides interactive visualizations and key performance indicators (KPIs) focused on compensation:

| Feature | Description | Key Metrics Displayed |
| :--- | :--- | :--- |
| **Median Salary Analysis** | View median compensation across major roles like **Data Scientist, Data Engineer, Senior Data Analyst,** and **Machine Learning Engineer**. | Overall Median Salary, Median Salary by Job Title (Ranked). |
| **Geographic Comparison** | Analyze salary differences across various countries, providing insight into global compensation parity. | Median Salary by **Country**, Ranked Country List. |
| **Employment Type Breakdown** | Compare compensation for different job schedules and types. | Median Salary by **Job Schedule Type** (Full-time, Contractor, Part-time, Internship, Temp work). |
| **Source Platform Analysis** | Identify the most common recruitment platforms and the volume of job posts. | Job Count by Source Platform (via LinkedIn, via Indeed, via ZipRecruiter, etc.). |
| **Interactive Filtering** | Use Slicers and Data Validation dropdowns to instantly filter the entire dashboard by Job Title, Country, and Employment Type. | N/A (User control feature). |

---

## 4. Data Source and Preparation

The dashboard is powered by a comprehensive dataset containing detailed job postings information.

### Data Fields
The raw data is structured with key fields including:
* `job_title_short` (Standardized role name)
* `job_country` (Geographical location of the job)
* `salary_year_avg` and `salary_hour_avg` (Annual and hourly average salary figures)
* `job_schedule_type` (Full-time, Contractor, etc.)
* `job_skills` (Required technical skills like 'python', 'sql', 'excel')

### Preparation Methodology
* **Data Cleaning:** Handling of missing values, standardization of job titles, and conversion of salary rates to a consistent annual average where possible.
* **Aggregation:** Extensive use of **Pivot Tables** and `GETPIVOTDATA` to summarize and calculate **median salaries** for all required dimensions (Title, Country, Type).
* **Lookups:** Utilization of functions like `VLOOKUP`/`XLOOKUP` and complex formulas to drive the dynamic calculations and KPI displays on the main dashboard sheet.

---

## 5. Technology and Tools

* **Core Technology:** **Microsoft Excel** (.xlsx)
* **Key Excel Components Used:**
    * **Pivot Tables & Pivot Charts:** For fast, complex data aggregation and visualization.
    * **Slicers:** For seamless, interactive filtering.
    * **Data Validation:** Used for creating user-friendly dropdown menus for filter selection.
    * **Advanced Formulas:** SUMIFS, AVERAGEIFS, MEDIAN, IF statements, and named ranges to link control elements to reporting metrics.

---
## 6. Snapshots 
Snapshot 1
<img width="1870" height="915" alt="Snapshot1" src="https://github.com/user-attachments/assets/bde1fdb9-b433-4a2c-abd8-d53b503497a4" />

## 7. How to Use the Dashboard

1.  **Download:** Clone this repository and open the **`Salary_Dashboard.xlsx`** file in Microsoft Excel (2016 or later recommended for full functionality).
2.  **Navigate:** Go to the main **`Dashboard`** sheet.
3.  **Filter:** Use the interactive **Slicers** (or dropdown menus powered by Data Validation) to select:
    * **Job Title:** e.g., "Data Scientist"
    * **Country:** e.g., "United States"
    * **Data Type:** e.g., "Contractor"
4.  **Analyze:** Observe how all charts, tables, and KPIs, including the **Data Science Salary Calculator**, instantly update to reflect the filtered data.

---

## 8. File Structure

The project is contained within a single Excel workbook, which is logically separated into multiple sheets for data integrity and presentation:

| Sheet Name (Derived from CSV) | Purpose |
| :--- | :--- |
| `Data` (`Salary_Dashboard.xlsx - Data.csv`) | The primary sheet containing the clean, raw job posting data. |
| `Dashboard` (`Salary_Dashboard.xlsx - Dashboard.csv`) | The main interactive interface for end-user analysis and visualization. |
| `Title_` (`Salary_Dashboard.xlsx - Title_.csv`) | Helper sheet for job title-specific aggregations and median salary calculations. |
| `Country` (`Salary_Dashboard.xlsx - Country.csv`) | Helper sheet for geographical (country-level) salary analysis. |
| `Type` (`Salary_Dashboard.xlsx - Type.csv`) | Helper sheet for job schedule type salary analysis. |
| `platform` (`Salary_Dashboard.xlsx - platform.csv`) | Helper sheet for analyzing job posting source platforms. |
| `Data_validation` (`Salary_Dashboard.xlsx - Data_validatation.csv`) | Lists and data used to populate dropdowns and slicers across the dashboard. |

---

**Thank you for checking out this project!** Feel free to fork the repository and explore the data.
