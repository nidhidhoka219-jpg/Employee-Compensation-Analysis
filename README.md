# Employee Compensation Analysis Dashboard (2011–2018)

## Project Overview
This project analyzes San Francisco employee compensation data to understand how pay, benefits, overtime, and job titles influence total compensation over time. The analysis combines Python based data cleaning and exploratory analysis with an interactive Power BI dashboard to help stakeholders track payroll growth, identify overtime heavy roles, and compare compensation across job families.

## Business Objective
The main goal is to turn raw compensation records into a decision support dashboard that answers these questions:

 - How has employee compensation changed from 2011 to 2018?
 - Which job titles receive the highest compensation?
 - Which roles depend most on overtime pay?
 - How do base pay, overtime, other pay, and benefits contribute to total compensation?
 - Where should management focus payroll control, workforce planning, and compensation review?


## Dataset Summary
- **Rows:** 312,882
- **Unique employees:** 130,283
- **Unique job titles:** 2,286
- **Time period:** 2011–2018

## Data Preparation
To make the dataset analysis ready, the following cleaning steps were required:
- Converted pay columns from mixed text/numeric format into numeric values.
- Treated **“Not Provided”** values as missing data.
- Standardized key text fields such as job titles and employee names.
- Used `Year` for trend analysis across 2011 - 2018.

### Data quality notes
- `BasePay` contains **606** “Not Provided” values.
- `Benefits` contains **36,160** “Not Provided” values.
- `Benefits` is completely unavailable for **2011** in this dataset, so benefit trend analysis starts effectively from 2012.

## Key KPIs
- **Average Total Pay:** 78,802.65
- **Average Total Compensation (with benefits):** 100,928.34
- **Total Payroll:** 24.66B
- **Total Compensation including benefits:** 31.58B
- **Total Benefits:** 6.92B

 ## Compensation Mix
  
  Average compensation is mainly driven by base pay and benefits:

  - Base Pay: ~69.2% of total compensation
  - Benefits: ~24.8%
  - Overtime Pay: ~5.6%
  - Other Pay: ~3.4%

## Yearly Trend
  - Average total pay increased from 71,744.10 in 2011 to 87,181.91 in 2018.
  -  Employee count also rose from 36,159 in 2011 to 42,309 in 2018.
  -  The pattern shows a sustained increase in payroll expense over the eight-year period.


### Notable Findings
**1. Payroll expanded steadily over time**

Average compensation increased across the 2011 – 2018 period, indicating continued payroll growth and a rising cost base for the city.

**2. Base pay is the core driver of compensation**

Base pay forms the largest share of total compensation, which means compensation planning should focus on base salary bands first, not only on overtime or bonuses.

**3. Benefits are a major budget component**

Benefits contribute nearly one-fourth of total compensation. Budget planning should therefore always be based on total compensation, not just salary.

**4. Certain roles are highly overtime dependent**

Roles in transit, maintenance, and operational support show strong overtime dependence. This usually points to staffing gaps, shift pressure, or coverage-heavy operations.

**5. Top paid roles are highly specialized**

The highest paying titles are concentrated in executive, investment, medical, and department head positions.

Examples of top average paying titles:

 - Chief Investment Officer
 - General Manager-Metropolitan Transit Authority
 - Physician Administrator, DPH
 - Managing Director
 - Chief, Fire Department

**6. Overtime heavy jobs are operational roles**

The highest overtime paying roles include:

 - Wire Rope Cable Maintenance Supervisor
 - Mech Shop & Equip Supt
 - Transit Power Line Sprv1
 - Trnst Power Line Wrk Sprv 2
 - Transportation Operations Spec

## Business Suggestions
### 1. Control overtime in high dependency roles
Roles such as transit operators, firefighters, deputy sheriffs, and similar operational jobs often show high overtime intensity. A review of shift design, staffing gaps, and leave coverage can reduce unnecessary overtime spend.

### 2. Use role-based compensation benchmarking
Average pay differs widely across job titles. Management should compare similar roles internally to identify underpaid, overpaid, or structurally inconsistent positions.

### 3. Review benefits cost growth annually
Benefits form a substantial part of total compensation. Annual benefit inflation should be tracked separately from salary increases so budget overruns can be caught early.

### 4. Separate strategic and operational payroll drivers
Senior leadership roles drive average compensation, while frontline roles drive headcount and overtime. These two cost centers should be monitored independently.


## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Power BI


## Files in this Repository
- `employee compensation data.csv` - Dataset
- `employee compensation analysis` - Pyhton notebook
- `san fransico.pbix` - Power BI dashboard file
- `README.md` - project overview and analysis summary

## Conclusion

This project provides a complete compensation intelligence view of San Francisco city payroll data from 2011 to 2018. It shows that payroll cost is mainly driven by base pay and benefits, while overtime remains a critical driver for specific operational roles.

