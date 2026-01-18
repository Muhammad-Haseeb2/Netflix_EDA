# Netflix Exploratory Data Analysis (EDA)

## Project Overview
This project performs **Exploratory Data Analysis (EDA)** on the Netflix titles dataset to understand content distribution, trends, and patterns available on the platform. The analysis focuses on cleaning raw data, handling multi-valued fields, visualizing key attributes, and extracting meaningful insights.

This notebook is designed as a **beginner-friendly EDA project**, suitable for academic submission and portfolio demonstration.

---

## Objectives
- Understand the structure and quality of the Netflix dataset
- Clean and preprocess missing, incorrect, and multi-valued data
- Analyze content distribution by type, country, rating, and genre
- Identify trends in content addition over time
- Generate clear visualizations and insights

---

## Dataset
- **Source:** Netflix Movies and TV Shows dataset (CSV format)
- **Key Columns:**
  - `type` – Movie or TV Show
  - `title` – Name of the content
  - `country` – Production country (multi-valued)
  - `date_added` – Date content was added to Netflix
  - `rating` – Content rating
  - `listed_in` – Genre (multi-valued)

---

## Tools & Libraries Used
- Python
- Pandas – data manipulation and cleaning
- Matplotlib – data visualization
- Seaborn – enhanced plotting (limited use)
- Jupyter Notebook

---

## Key Steps Performed

### 1. Data Loading & Inspection
- Loaded the CSV file into a Pandas DataFrame
- Inspected data using `.head()`, `.info()`, and `.describe()`

### 2. Data Cleaning
- Converted `date_added` column to datetime format
- Handled missing values
- Processed multi-valued columns (`country`, `listed_in`) using `split()` and `explode()`

### 3. Exploratory Analysis
- Movies vs TV Shows distribution
- Top 10 content-producing countries
- Content rating distribution
- Most common genres
- Year-wise content addition trends

### 4. Visualization
- Bar charts for categorical comparisons
- Trend analysis over time
- Simple, readable plots suitable for academic grading

---

## Key Insights
- Netflix hosts more **Movies** than TV Shows
- The **United States** dominates content production
- A significant portion of content is rated **TV-MA**, indicating mature content
- Content addition increased rapidly after **2016**, reflecting Netflix’s global expansion
- Drama and International content are among the most common genres

---

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/Muhammad-Haseeb2/Netflix-EDA.git
   ```
2. Navigate to the project directory
3. Open the notebook:
   ```bash
   jupyter notebook
   ```
4. Run all cells sequentially

---

## Project Status
✔ Completed basic EDA
✔ Clean and readable visualizations
✔ Suitable for beginner-level data analysis portfolio

---

## Author
**Muhammad Haseeb**  
Bachelor’s Student – Artificial Intelligence

---

## License
This project is for educational purposes only.

