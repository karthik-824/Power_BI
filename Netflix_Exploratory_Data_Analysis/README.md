# 🎬 End-to-End Data Analysis of Netflix Movies and TV Shows

##  Project Overview
This project focuses on cleaning, transforming, and analyzing the Netflix titles dataset to understand what type of content Netflix offers. The dataset from Kaggle contains **8,807 titles** with details like type, director, cast, country, and description.

**Dataset:** https://www.kaggle.com/datasets/shivamb/netflix-shows/data  
**Tools Used:** Microsoft Excel, Power BI Desktop, Power Query  

---

##  Data Cleaning & Transformation

###  Data Profiling
- Checked dataset quality using Power Query tools.  
- Found many missing values in the **Director** column (31%).  
- Noticed uneven data in the **Country** column.

###  Fixing Errors
- Found a row where **Type** was incorrectly shown as `"William Wyler"` due to CSV formatting issues.
- Corrected the row using Power Query.

###  Handling Missing Values
- Filled missing **Director** values with `"Director Missing"`.  
- Filled missing **Country** values with `"United States"` (most common country at 31%).

###  Date Formatting
- Converted `date_added` into proper Date format using **Using Locale** to avoid regional date errors.

###  Feature Engineering
- Split **Duration** into numeric values for movies (minutes) and TV shows (seasons).
- Split **Genres** (listed_in) into separate rows to analyze each genre individually.

###  Text Search
- Converted descriptions to lowercase.
- Used keywords like “murder,” “death,” and “kill” to find **Murder Mystery** content.

---

##  Key Insights

###  Content Type Breakdown
- **Movies:** ~68%  
- **TV Shows:** ~32%  

###  Duration
- Most movies were **90 minutes** long.

###  Top Countries
1. United States – 31%  
2. India – 11%  
3. United Kingdom – 4%  

---

##  Skills Demonstrated

### Power Query
- Data cleaning and transformation  
- Handling missing values  
- Splitting and reshaping columns  
- Fixing CSV errors  

### Data Quality
- Full dataset profiling  
- Identifying data shift issues

### Data Modeling
- Creating dimension tables  
- Building one-to-many relationships for clean Power BI models  

---
