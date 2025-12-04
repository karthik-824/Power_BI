
# 🎬 End-to-End Data Analysis of Netflix Movies and TV Shows

##  Project Overview
**End-to-End Data Analysis of Netflix Movies and TV Shows**  
**Description:**  
This project focuses on cleaning, transforming, and analyzing the Netflix titles dataset to perform Exploratory Data Analysis (EDA) and uncover meaningful content trends.

**Dataset Source:**  
A publicly available Kaggle dataset containing **8,807 rows** of Netflix titles, including features such as type, title, director, cast, country, release year, and description.

https://www.kaggle.com/datasets/shivamb/netflix-shows/data

**Tools Used:**  
- Microsoft Excel  
- Power BI Desktop  
- Power Query  

---

##  Data Cleaning & Transformation (Power Query)

###  Data Profiling
- Utilized Power Query’s **Column Quality, Column Distribution, and Column Profile** tools to assess dataset health.  
- Identified:
  - High missing values in the **Director** column (~31%).  
  - Uneven distribution patterns in the **Country** column.

###  Fixing Data Shift / Parsing Errors
- Detected a CSV formatting issue where the **Type** column incorrectly contained a value `"William Wyler"` due to misplaced commas and newline characters.
- Corrected the row-level data shift using Power Query transformations.

### Handling Missing Values (Imputation)
- **Director:** Replaced all nulls with `"Director Missing"` to support explicit filtering in visuals.  
- **Country:** Imputed missing values using a **Most Popular Country Strategy**, replacing blanks with `"United States"` (the top content producer at 31%).

###  Date Normalization
- Converted `date_added` from text to a proper **Date** format.
- Used **“Using Locale”** to correctly parse dates regardless of system region settings (avoiding MM/DD vs. DD/MM conflicts).

###  Feature Engineering
- **Duration Standardization (Movies vs. TV Shows):**  
  Created conditional columns to separate numeric values (minutes for movies, seasons for TV shows).
  
- **Genre Expansion for Analysis:**  
  - The `listed_in` column contained comma-separated genres (e.g., `"International, Dramas"`).  
  - Created a duplicate table and **split genres into rows** to support granular genre analysis.

### Text Mining
- Standardized descriptions to lowercase and built keyword search logic to identify **"Murder Mystery"** content by scanning for keywords such as:
  - "murder"
  - "death"
  - "kill"

---

##  Key Insights from Power BI Visualizations

###  Content Distribution
- **Movies:** ~68%  
- **TV Shows:** ~32%  

###  Duration Trends
- The most common movie duration in the dataset was **90 minutes**.

###  Top Content-Producing Countries
1. **United States – 31%**  
2. **India – 11%**  
3. **United Kingdom – 4%**

---

##  Technical Skills Demonstrated

###  Power Query
- Advanced data transformation  
- Conditional logic  
- Column splitting & normalization  
- Handling CSV parsing errors  
- Using “M” language through the UI

###  Data Quality & Profiling
- Column profiling on the **entire dataset**, not just the previewed rows  
- Detection of anomalies and data shifts

###  Data Modeling
- Built separate **dimension tables** (e.g., Category Dimension for genres)  
- Established **one-to-many relationships** to support clean Power BI modeling

---

