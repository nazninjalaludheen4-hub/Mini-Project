# UDISE Schools Mini Project

## Project Description
This mini project analyzes school infrastructure data from the UDISE+ dataset using Power BI and Excel.
The goal is to visualize school distribution, enrollment patterns, and infrastructure gaps across rural and urban areas.

## Dataset
- **Source**: UDISE+ Schools Sample Dataset
- **File**: `SCHOOLS SAMPLE.xlsx`
- **Records**: 501 schools
- **Key Columns**: state_name, district_name, location_type, class_students, year_of_establishment, school_category, management

## Tools Used
- **Power BI Desktop** – DAX measures, dashboards
- **Excel** –  Data cleaning,Pivot tables, 
- **GitHub** – Project documentation and submission

## Key Visualizations
1. **KPI Cards**: Total Schools, Total Students, % Rural Schools
2. **Donut Chart**: Schools by Category
3. **Scatter Chart**: School Age vs Enrollment
4. **Bar Chart**: Schools by Management Type


## DAX Measures Created
```DAX
Total Schools = COUNTROWS(SCHOOLS SAMPLE)
Total Students = SUM('SCHOOLS SAMPLE'[class_students])
% Rural Schools = DIVIDE(COUNTROWS(FILTER('SCHOOLS SAMPLE', 'SCHOOLS SAMPLE'[location_type] = "Rural")), [Total Schools])


