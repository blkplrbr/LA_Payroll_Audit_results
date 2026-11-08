# Los Angeles City Payroll Audit & Data Cleanup

## Project Overview
This project involved auditing a massive, raw municipal payroll dataset (Los Angeles city employees) to identify the highest-paid departments in preparation for a simulated city budget cut. The goal was to determine which department consumed the most financial resources.

## The Problem
The raw dataset was incredibly large and contained significant data integrity issues (duplicate entries, trailing spaces, inconsistent formatting). Manipulating the data before cleaning it would have resulted in inaccurate financial reporting. Furthermore, the file size was too large for standard uploads/dashboards, requiring optimization.

## The Solution (Methodology)

**Step 1: Establishing the Standard Operating Procedure (SOP)**
Before analysis, I developed a standardized data-cleaning workflow. The rule was: *"Clean first, analyze second."* 
*   Used `TRIM` functions to remove invisible trailing spaces that break VLOOKUPs and Pivot Tables.
*   Removed duplicate records to ensure each employee was only counted once.
*   Standardized text formatting (e.g., capitalization).

**Step 2: Data Optimization**
*   Because the original file was too large for standard presentation, I created a compressed "small version" to optimize performance without losing critical data points. 

**Step 3: Analysis & Visualization**
*   Imported the cleaned data and created **Pivot Tables** aggregating total payroll costs by department.
*   Generated a **Pie Chart** to visually represent the budgetary distribution and identify the largest cost center (the department that would be hit hardest by a budget cut).

## Business Impact
*   Transformed a messy, unusable dataset into a clean, reliable financial report.
*   Provided clear, visual data (Pivot Tables/Charts) that allowed stakeholders to immediately identify the most expensive city departments.
*   Established a reusable data-cleaning SOP that can be applied to future client datasets.

## Tools Used
*   Microsoft Excel (TRIM, Remove Duplicates, Pivot Tables, Charts)
*   Data source: Kaggle (Los Angeles City Payroll)
