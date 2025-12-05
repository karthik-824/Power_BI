#  Employee Attendance & Productivity Dashboard 

<img width="1157" height="651" alt="Screenshot 2025-12-05 120813" src="https://github.com/user-attachments/assets/3364b0f6-533f-4a51-96b2-76ec69e7221b" />


## Project Overview
This project transforms non-normalized attendance data into an interactive Power BI dashboard.  
The goal was to recreate a pixel-perfect, app-like UI (inspired by a Tableau design) using **custom SVG visuals** and **advanced DAX**.

The dashboard tracks attendance for **25 employees**, showing workdays, sick leave, holidays, and productivity trends.

---

##  Key Features
- **Custom SVG Calendar View**  
  Day-by-day attendance shown using SVG shapes (Green = Present, Yellow = Weekend, Red = Sick/Holiday).

- **Employee Cards With Photos**  
  Employee details and profile images rendered directly inside Power BI.

- **Smart KPIs**  
  Automatic calculations for Attendance %, Total Days, Working Days, and Monthly metrics.

---

##  Dataset
- Excel attendance matrix (Employees as columns, Dates as rows)  
- Employee table containing names and profile image URLs  

**Tools Used:** Power BI • Power Query • DAX • Excel 

---

##  Key Insights
- **Attendance Rate:** ~88% overall  
- **Workforce Capacity:** ~3,000 total days vs. ~2,000 attended  
- Calendar visual helps spot patterns such as long sick leave streaks or weekend clusters.  

---

##  Skills Demonstrated
**Power Query**
- Unpivoting and reshaping data    
- Calendar logic and custom columns  

**DAX**
- Building SVG visuals inside measures  
- Dynamic formatting (colors, shapes, text)  
- KPIs using `CALCULATE`, `VAR`, and context transition
  
---

