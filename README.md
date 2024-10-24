# HR-Analytics-Power-BI-Project
## Overview
This repository contains the HR Analytics project developed in Power BI. The project aims to analyze employee attendance data, focusing on key metrics such as total working days, present days, Work-from-Home (WFH) days, and Sick Leave (SL) days. It includes data gathering, transformation, and the creation of interactive dashboards to visualize attendance patterns.

## Project Workflow
### 1. Data Gathering and Transformation
Data Source: Attendance data is collected from Excel files containing multiple sheets.  
Power Query Editor: Imported attendance data into Power BI using Power Query Editor.
Selected only one relevant sheet and unpivoted columns to structure the data in the required format.
### 2. Data Transformation
Parameter and Function: Created a parameter to dynamically reference different sheets in the workbook.  
Built a custom function based on the parameter to apply transformations to the rest of the attendance sheets.

### 3. Data Cleaning
Removed unnecessary columns from the dataset.Loaded the cleaned and transformed data into Power BI for analysis.

### 4. New Table Creation and DAX Measures
Created a new table to store calculated measures for analysis.  
Used DAX (Data Analysis Expressions) formulas to add key metrics such as:  
Total Working Days  
Total Present Days  
Present Percentage  
WFH Percentage  
Sick Leave Percentage  

### 5. Additional Data Columns
Added new calculated columns in the attendance dataset for:  
WFH (Work From Home) Count  
SL (Sick Leave) Count  
### 6. DAX Measures for Attendance Analysis
Defined the following DAX measures:  
Total Working Days: Total days in the attendance period.  
Total Present Days: Sum of all present days for each employee.  
Present Percentage: (Total Present / Total Working Days) * 100  
WFH Percentage: (Sum of WFH Days / Total Present) * 100  
SL Percentage: (Sum of SL Days / Total Working Days) * 100  
Included slicers for filtering by month, providing an interactive way to view attendance trends for each month.

### 7. Dashboard Creation
Built a comprehensive dashboard to visualize key attendance metrics:  
Area Charts for:  
Present days by date  
WFH days by date  
SL days by date  
A table view showing employees' names and their attendance values.  
### 8. Additional Analysis Tables
Created two additional tables for detailed analysis:  
Day and Present Percentage: Displays the present percentage for each day.  
Day and Sick Leave Percentage: Displays the SL percentage for each day.  
## Dashboard Highlights
Present Percentage: Formula - (Total Present / Total Working Days) * 100  
WFH Percentage: Formula - (Sum(WFH Days) / Total Present Days) * 100  
SL Percentage: Formula - (Sum(SL Days) / Total Working Days) * 100  
The dashboard helps the HR team monitor attendance trends over time, evaluate WFH and SL percentages, and understand the overall employee presence at a glance.

## How to Use
Clone the repository to your local machine.  
Open Power BI Desktop and load the .pbix file.  
Interact with the slicers and visuals to explore the attendance data.  
## Requirements
Power BI Desktop (Latest Version)
## License
This project is licensed under the MIT License - see the LICENSE file for details.
