# HR DataForge – Multi-Workbook HR Data Cleaning & Workforce Analysis Using Power Query

## 📌 Project Overview

**HR DataForge** is an end-to-end HR data cleaning, transformation, consolidation, and workforce analysis project developed using **Microsoft Excel, Power Query, and PivotTables**.

The project works with **5 monthly HR Excel workbooks** containing employee-level records. The objective was to combine the monthly files into one reliable master dataset, clean and standardize the data, validate data quality, create calculated fields, and build multiple workforce analysis reports.

The project demonstrates a complete **ETL (Extract, Transform, Load)** workflow using Power Query, followed by multidimensional HR analysis using Excel PivotTables.

### Project Flow

**5 Monthly HR Workbooks → Power Query → Data Cleaning → Data Transformation → Data Validation → Master Dataset → PivotTable Analysis → HR Reporting**

---

## 📊 Project Snapshot

| Category               | Details                                                                                |
| ---------------------- | -------------------------------------------------------------------------------------- |
| **Project Type**       | HR Data Cleaning & Workforce Analysis                                                  |
| **Tools Used**         | Microsoft Excel, Power Query, PivotTables                                              |
| **Source Files**       | 5 Monthly HR Excel Workbooks                                                           |
| **Raw Records**        | 51,000+                                                                                |
| **Clean Records**      | 50,750                                                                                 |
| **Primary Identifier** | Employee_ID                                                                            |
| **Data Processing**    | ETL, Cleaning, Transformation & Validation                                             |
| **Analysis**           | Department, Job Role, Manager, Performance, Experience, Shift, Location, State & Month |
| **Final Output**       | Clean Master Dataset + Multi-Dimensional HR Analysis                                   |

---

# 📁 1. Project Tasks & Objectives

The first stage was to define the overall project requirements and establish a structured workflow for handling multiple HR workbooks.

The major objectives were:

* Consolidate multiple monthly HR workbooks.
* Create a single employee-level master dataset.
* Remove unnecessary and duplicate records.
* Standardize inconsistent text values.
* Handle missing and non-applicable values.
* Validate employee information.
* Standardize data types.
* Create calculated HR metrics.
* Perform workforce analysis.
* Build PivotTable-based HR reports.
* Create a scalable Power Query workflow that can be refreshed when new monthly data is added.

![Project Tasks](Images/1.png)

---

# 📂 2. Source HR Dataset

The project started with multiple monthly Excel workbooks containing HR employee records.

The monthly files represented different reporting periods, including:

* January 2026
* February 2026
* March 2026
* April 2026
* May 2026

Each workbook contained employee information such as:

* Employee ID
* Employee Name
* Department
* Job Role
* Joining Date
* Salary
* Bonus
* Location
* State
* Manager
* Shift
* Performance
* Experience
* Attendance
* Email
* Other HR attributes

The objective was to transform these separate monthly files into one standardized dataset.

![Source Dataset](Images/2.png)

---

# 🔄 3. Combining Multiple Workbooks Using Power Query

Power Query was used to create a folder-based data-import workflow.

Instead of manually opening and copying data from each workbook, the files were connected through Power Query and combined into a centralized dataset.

The workflow included:

1. Connecting to the folder containing the HR workbooks.
2. Reading the available Excel files.
3. Extracting the required workbook data.
4. Combining the monthly datasets.
5. Expanding the employee records.
6. Creating one consolidated dataset.

This approach makes the process more scalable because new monthly workbooks can be added to the source folder and the query can be refreshed.

![Power Query Import](Images/3.png)

---

# ⚙️ 4. Power Query Data Transformation

After importing the workbooks, Power Query was used as the main transformation layer.

The transformation process included:

* Removing unnecessary rows.
* Removing temporary information.
* Removing repeated headers.
* Promoting the correct headers.
* Standardizing column names.
* Cleaning text values.
* Correcting inconsistent values.
* Replacing invalid values.
* Handling missing values.
* Changing data types.
* Creating calculated columns.
* Sorting and grouping records.

This created a structured and analysis-ready master dataset.

![Power Query Transformation](Images/4.png)

---

# 🧹 5. Data Cleaning & Query Transformation

The raw employee data contained several common data-quality issues.

Power Query transformations were applied to standardize the dataset.

### Cleaning activities included:

* Trimming unnecessary spaces.
* Standardizing capitalization.
* Correcting inconsistent spellings.
* Replacing incorrect categorical values.
* Standardizing Department names.
* Standardizing Job Roles.
* Standardizing Location and State.
* Cleaning Manager names.
* Standardizing Shift values.
* Standardizing Performance categories.
* Handling blank and null values.
* Identifying duplicate Employee IDs.
* Converting columns to appropriate data types.

![Clean Data](Images/5.1.png)

### Additional Power Query Processing

Additional transformations were performed to prepare the final dataset for analysis.

These included grouping, sorting, calculated columns, value replacement, and restructuring of the data.

![Power Query Data Processing](Images/5.2.png)

---

# 🧪 6. Data Quality & Validation

Power Query's **Column Quality** functionality was used to evaluate the quality of the dataset.

The dataset was reviewed for:

* Valid values
* Error values
* Empty values
* Null values
* Missing information
* Incorrect formats
* Invalid email records
* Duplicate records
* Incorrect data types

Where information was genuinely unavailable, values were standardized using appropriate classifications such as:

**Missing** / **Not Available**

This prevented unavailable information from being confused with actual business values.



---

# 📊 7. Workforce Analysis Preparation

After cleaning and validation, the master dataset was prepared for workforce analysis.

Calculated and standardized fields included:

### Total Compensation

**Total Compensation = Salary + Bonus**

This metric was created to evaluate the overall compensation associated with employees.

### Month-wise Analysis

A Month-wise field was also created from workbook names such as:

* January 2026
* February 2026
* March 2026
* April 2026
* May 2026

This enabled monthly workforce comparisons.



---

# 🏢 8. Department-wise Analysis

A Department-wise analysis was created to understand workforce distribution across departments.

The analysis included:

* Employee Count
* Average Salary
* Average Bonus
* Job Roles
* Total Compensation

The departments analyzed included areas such as:

* Finance
* HR
* IT
* Marketing
* Operations
* Sales
* Missing / Not Available

![Department-wise Analysis](Images/6.png)

---

# 💼 9. Job Role-wise Analysis

Job Role data was analyzed to understand the distribution of employees across different positions.

The analysis included roles such as:

* Account Manager
* Accountant
* Business Development Executive
* Data Analyst
* HR Analyst
* HR Manager
* Marketing Analyst
* Operations Analyst
* Sales Manager
* Software Engineer
* Power BI Developer
* QA Engineer
* System Administrator

Job roles were grouped and standardized to make the analysis consistent.

![Job Role Analysis](Images/6.png)

---

# 👨‍💼 10. Manager-wise Analysis

Manager-wise analysis was created to evaluate workforce distribution and compensation across managers.

The analysis included:

* Manager
* Employee Count
* Total Compensation

This provides a management-level view of employee distribution and compensation.

![Manager-wise Analysis](Images/9.png)

---

# 🔄 11. Shift-wise Analysis

Employee records were analyzed according to working shifts.

The analysis covered:

* Morning
* Evening
* Night
* General

Key metrics included:

* Employee Count
* Total Compensation
* Workforce distribution

This helps understand how employees and compensation are distributed across different working shifts.

![Shift-wise Analysis](Images/12.png)

---

# ⭐ 12. Performance-wise Analysis

Employee performance categories were analyzed to compare workforce distribution and HR metrics.

The performance categories included:

* Excellent
* Very Good
* Good
* Average
* Needs Improvement

The analysis included:

* Employee Count
* Average Salary
* Average Bonus
* Attendance

![Performance Analysis](Images/10.png)

---

# 📈 13. Experience-wise Analysis

Experience-level analysis was created to understand workforce distribution across different experience groups.

Experience categories included:

* 0 years
* 1 year
* 2 years
* 3 years
* 4 years
* 5 years

The analysis included:

* Employee Count
* Total Compensation
* Attendance

![Experience Analysis](Images/7.png)

---

# 📍 14. Location & State-wise Analysis

Location and State information was analyzed to understand geographical workforce distribution.

The analysis included locations such as:

* Bengaluru
* Chennai
* Delhi
* Gurgaon
* Hyderabad
* Jaipur
* Kolkata
* Mumbai
* Noida
* Pune

State-level information was also included.

Where location information was not available, the records were consolidated under a standardized **Not Available** category while preserving the available State information.

![Location and State Analysis](Images/8.png)

---

# 📥 15. Loading the Clean Master Dataset into Excel

After completing the Power Query transformations, the final cleaned dataset was loaded into Excel.

The master dataset contained **50,750 clean employee records**.

The loaded data was then used as the foundation for the PivotTable-based workforce analysis.

![Loaded Clean Dataset](Images/5.png)

![Loaded Clean Dataset](Images/3.png)

---

# 📋 16. PivotTable Analysis

Excel PivotTables were created to convert the cleaned employee-level data into summarized HR reports.

The PivotTables provided a structured view of workforce metrics without modifying the underlying master dataset.

The analysis covered multiple HR dimensions.

![PivotTable Analysis](Images/15.1.png)

---

# 👨‍💼 17. Manager PivotTable

A dedicated Manager PivotTable was created to analyze employee distribution and compensation by manager.

### Metrics:

* Manager
* Employee Count
* Total Compensation

This helps identify the workforce size and compensation associated with each manager.

![Manager PivotTable](Images/16.png)

---

# 👥 18. Employee & Workforce Analysis

Employee-level workforce summaries were created using PivotTables.

The analysis provides a high-level view of employee counts and workforce-related metrics across different categories.

![Employee Analysis](Images/18.png)

---

# 🕐 19. Shift PivotTable

A Shift PivotTable was created to analyze employees according to their working shifts.

### Shift categories:

* Morning
* Evening
* Night
* General

### Metrics:

* Employee Count
* Total Compensation

![Shift PivotTable](Images/19.png)

---

# 🏢 20. Department PivotTable

The Department PivotTable provides a summarized view of the workforce by department.

### Metrics:

* Employee Count
* Average Salary
* Average Bonus
* Job Roles

This allows departments to be compared using standardized workforce metrics.

![Department PivotTable](Images/20.png)

---

# 📍 21. Location PivotTable

A Location PivotTable was created to summarize employee distribution and compensation by location.

### Metrics:

* Location
* State
* Employee Count
* Total Compensation

![Location PivotTable](Images/21.png)

---

# ⭐ 22. Performance PivotTable

A Performance PivotTable was created to analyze employee performance categories.

### Metrics:

* Performance
* Employee Count
* Average Salary
* Average Bonus
* Attendance

This provides a summarized view of workforce performance and related HR metrics.

![Performance PivotTable](Images/17.png)

---

# 📊 23. Complete HR Analysis Dashboard Structure

The completed workbook contains multiple analytical sections covering:

* Department
* Job Role
* Manager
* Experience
* Shift
* Performance
* Location
* State
* Month

These reports provide different perspectives of the same cleaned master dataset.

![HR Analysis](Images/23.png)

---

# 📅 24. Month-wise Workforce Analysis

A Month-wise field was created from the source workbook names.

This allows the HR dataset to be analyzed across monthly reporting periods.

### Monthly periods:

**January 2026 → February 2026 → March 2026 → April 2026 → May 2026**

The month field makes it possible to compare workforce metrics across reporting periods.

![Month-wise Analysis](Images/24.png)

---

# 🔁 25. Adding a New Monthly Workbook

One of the important advantages of the folder-based Power Query workflow is its ability to handle new monthly files.

A new HR workbook can be placed into the source folder without manually rebuilding the entire dataset.

The Power Query workflow can then be refreshed to incorporate the new records.

![Adding New Workbook](Images/21.png)

---

# 🔄 26. Refreshing the Power Query Workflow

After adding the new workbook, the Power Query process was refreshed.

The query automatically processed the new source file using the existing transformation steps.

This demonstrates that the project is not only a one-time data-cleaning exercise but also a **repeatable and scalable ETL workflow**.

![Refresh Query](Images/22.png)

---

# ✅ 27. Updated Clean Dataset

After refreshing the query, the new records were incorporated into the consolidated master dataset.

The same cleaning and transformation rules were automatically applied to the newly added data.

This ensures consistency between historical and newly added monthly records.

![Updated Clean Data](Images/27.png)

---

# 📈 28. Final HR Reporting Output

The final output combines the cleaned master dataset with multiple workforce analyses.

The completed reporting structure provides HR insights across:

* Department
* Job Role
* Manager
* Performance
* Experience
* Shift
* Location
* State
* Month
* Employee Count
* Salary
* Bonus
* Attendance
* Total Compensation

The project demonstrates how raw multi-workbook HR data can be converted into a structured, validated, and analysis-ready workforce reporting solution.

![Final HR Reporting](Images/28.png)

---

# 🔄 End-to-End Workflow

```text
Monthly HR Excel Workbooks
          ↓
     Folder Import
          ↓
      Power Query
          ↓
 Combine & Expand Data
          ↓
 Remove Unwanted Rows
          ↓
 Promote Headers
          ↓
 Remove Duplicates
          ↓
 Clean & Standardize Data
          ↓
 Handle Missing Values
          ↓
 Validate Data Quality
          ↓
 Standardize Data Types
          ↓
 Create Total Compensation
          ↓
 Create Month-wise Field
          ↓
 Clean Master Dataset
          ↓
 Load into Excel
          ↓
 Create PivotTables
          ↓
 HR Workforce Analysis
          ↓
 Reporting & Insights
```

# 🛠️ Tools & Technologies

* **Microsoft Excel**
* **Power Query**
* **Excel PivotTables**
* **Power Query Column Quality**
* **Power Query Transformations**
* **Data Cleaning & Standardization**
* **ETL Workflow**
* **HR Workforce Analytics**

# 📌 Key Skills Demonstrated

* Multi-workbook data consolidation
* Folder-based Power Query automation
* Data cleaning
* Data transformation
* Duplicate removal
* Missing-value handling
* Data validation
* Data type standardization
* Text standardization
* Calculated columns
* Total Compensation calculation
* Month-wise data preparation
* Group By operations
* PivotTable analysis
* Workforce analytics
* HR reporting
* Scalable data-refresh workflow

# 🏆 Project Outcome

**51,000+ raw HR records were transformed into 50,750 clean employee records and converted into a validated, analysis-ready master dataset with multi-dimensional workforce reporting across Department, Job Role, Manager, Performance, Experience, Shift, Location, State, and Month.**
