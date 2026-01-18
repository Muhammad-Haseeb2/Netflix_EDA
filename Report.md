# Netflix Dataset – Exploratory Data Analysis Report

## 1. Introduction
This report presents a complete exploratory data analysis (EDA) of a Netflix dataset containing information about movies and TV shows available on the platform. The purpose of this analysis was to understand the structure of the dataset, clean data quality issues, explore patterns, and extract meaningful insights using visual analysis.

This document focuses on the **story of the data**, while all implementation details, code, and plots are available in the accompanying Jupyter Notebook.

---

## 2. Dataset Overview
The dataset consists of records related to Netflix titles with multiple attributes describing each title.

Key columns used in this analysis include:
- **type** – Movie or TV Show  
- **title** – Name of the content  
- **country** – Country of production  
- **date_added** – Date when the content was added to Netflix  
- **release_year** – Year the content was released  
- **rating** – Content rating (e.g., PG, R, TV-MA)  
- **listed_in** – Genre(s)  
- **duration** – Length of the content  

The dataset contained missing values and multi-valued columns, which required cleaning before analysis.

---

## 3. Data Issues Identified
During initial inspection, the following issues were found:

1. **Missing Values**  
   - Some records had missing values in `country` and `date_added`.

2. **Multi-valued Columns**  
   - Columns such as `country` and `listed_in` contained multiple values separated by commas.

3. **Incorrect Data Types**  
   - The `date_added` column was stored as text instead of a datetime format.

4. **Duplicate Records**  
   - Duplicate titles existed that could distort analysis results.

---

## 4. Data Cleaning Process
To address these issues, the following steps were taken:

- Missing country values were filled with `"Unknown"`.
- `date_added` was converted to a datetime format for time-based analysis.
- Multi-valued columns (`country` and `listed_in`) were split and exploded so each row contained a single value.
- Duplicate records were removed to avoid double counting.

After cleaning, the dataset was in a structured and analysis-ready form.

---

## 5. Analysis Approach
The analysis focused on answering the following questions:

- What is the distribution of Movies vs TV Shows on Netflix?
- Which countries produce the most Netflix content?
- What are the most common genres?
- How have content ratings changed over time?
- How has Netflix’s content library grown over the years?

Bar charts and line plots were used to visually analyze trends and distributions.

---

## 6. Visual Analysis Summary
The following visualizations were created in the analysis notebook:

- **Movies vs TV Shows distribution**
- **Top 10 countries by number of titles**
- **Top genres on Netflix**
- **Content rating trends over years**
- **Growth of Netflix titles over time**

Each plot helped reveal trends that are discussed in the insights section below.

---

## 7. Key Insights
- Movies dominate Netflix’s catalog, though TV Shows have been increasing steadily.
- The United States is the largest producer of Netflix content, followed by India and the United Kingdom.
- Drama and Comedy are the most common genres on the platform.
- Mature-rated content (such as TV-MA and R) has increased over recent years.
- Netflix’s library has grown consistently over time, reflecting the platform’s expansion.

---

## 8. Conclusion
This EDA project demonstrates the complete data analysis workflow, starting from raw data inspection to cleaning, visualization, and insight generation. By separating analysis code from this written report, the project clearly communicates both the **technical work** and the **data story**.

The findings provide a clear overview of Netflix’s content distribution and growth patterns, making this analysis useful for understanding trends in streaming content.