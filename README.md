# 🏢 HR DATAFORGE — Multi-Workbook HR Data Cleaning & Workforce Analysis Using Power Query

> **An end-to-end HR data cleaning, transformation, consolidation, validation, and workforce analysis project using Microsoft Excel, Power Query, and PivotTables.**

---

## 📌 Project Overview

This project demonstrates an end-to-end **HR Data Cleaning and Workforce Analysis workflow** using **Microsoft Excel and Power Query**.

The project started with multiple monthly HR Excel workbooks containing employee-level records. Instead of manually opening, cleaning, and combining every workbook, **Power Query** was used to create a repeatable data transformation workflow.

The five monthly HR workbooks were consolidated into a single master dataset, followed by extensive data cleaning, standardization, validation, transformation, and calculated-field creation.

After the Power Query transformation process was completed, the cleaned dataset was loaded back into Excel and used to create multiple **section-wise PivotTable analyses**.

The final analysis covers:

🔹 Department & Job Role  
🔹 Manager  
🔹 Experience  
🔹 Shift  
🔹 Performance  
🔹 Location & State  
🔹 Month-wise workforce information  
🔹 Employee Count  
🔹 Salary  
🔹 Bonus  
🔹 Attendance  
🔹 Total Compensation  

The overall workflow can be summarized as:

**Raw HR Workbooks → Power Query → Data Cleaning → Data Transformation → Validation → Clean Master Dataset → Load to Excel → PivotTables → Workforce Analysis**

---

## 🎯 Project Objective

The main objective of this project was to:

🔹 Consolidate multiple monthly HR Excel workbooks into one master dataset.

🔹 Clean and standardize inconsistent employee data using Power Query.

🔹 Remove duplicate, unnecessary, temporary, and repeated records.

🔹 Handle missing, blank, null, and non-applicable values appropriately.

🔹 Standardize categorical fields such as Department, Job Role, Location, State, Manager, Shift, and Performance.

🔹 Convert fields into appropriate data types.

🔹 Validate employee email records and identify invalid values.

🔹 Create calculated fields such as **Total Compensation**.

🔹 Create a **Month-wise** field from monthly workbook names.

🔹 Load the final cleaned dataset into Excel.

🔹 Create multiple PivotTables for workforce analysis and reporting.

---

## 🛠️ Tools & Technologies Used

🔹 **Microsoft Excel**

🔹 **Power Query**

🔹 **Excel PivotTables**

🔹 **Power Query Column Quality**

🔹 **Power Query Data Transformation**

🔹 **Power Query Group By**

🔹 **Folder-Based Data Consolidation**

---

# 📂 Source Data

The project uses **5 monthly HR Excel workbooks** stored in a folder.

The monthly files follow a naming structure similar to:

```text
01_January_2026.xlsx
02_February_2026.xlsx
03_March_2026.xlsx
04_April_2026.xlsx
05_May_2026.xlsx
