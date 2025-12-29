# Excel Payroll Automation Project

## Project Overview
This project demonstrates a complete payroll calculation system built using Microsoft Excel.  
The workbook calculates employee pay based on hourly wages, hours worked, overtime hours, overtime bonuses, weekly total pay, and monthly payroll totals for January.

The goal of this project is to showcase:
- Excel formula skills
- Payroll logic implementation
- Overtime and bonus calculations
- Clean, structured spreadsheet design
- Business-ready reporting

---

## Sheet 1: Payroll
**Purpose:**  
Calculate basic weekly pay for each employee using hourly wage and hours worked.

**Columns Explained:**
- Last Name
- First Name
- Hourly Wage
- Hours Worked
- Pay

**Logic Used:**
- Pay is calculated by multiplying hourly wage by hours worked.

**Formula Example:**
Pay = Hourly Wage × Hours Worked


This sheet forms the foundation of the payroll system.

---

## Sheet 2: Overtime = Bonus
**Purpose:**  
Extend the payroll by calculating overtime hours, overtime bonus, and total weekly pay.

**Key Columns:**
- Hours Worked
- Overtime Hours
- Pay
- Overtime Bonus
- Total Pay

**Logic Used:**
- Overtime hours are calculated when hours worked exceed 40.
- Overtime bonus is calculated at 0.5× hourly wage per overtime hour.
- Total Pay = Regular Pay + Overtime Bonus

**Key Formulas:**
Overtime Hours = IF(Hours Worked > 40, Hours Worked - 40, 0)
Pay = Hourly Wage × Hours Worked
Overtime Bonus = 0.5 × Hourly Wage × Overtime Hours
Total Pay = Pay + Overtime Bonus


This sheet introduces conditional logic and bonus modeling.

---

## Sheet 3: January Payroll
**Purpose:**  
Calculate payroll across multiple weeks in January and generate a monthly total for each employee.

**Weekly Structure:**
- Weekly Hours Worked (01-Jan, 08-Jan, 15-Jan, 22-Jan, 29-Jan)
- Weekly Overtime Hours
- Weekly Pay
- Weekly Overtime Bonus
- Weekly Total Pay

**Monthly Calculation:**
- January Pay is calculated by summing all weekly total pay values.

**Key Formula Example:**
January Pay = SUM(Weekly Total Pay Columns)


This sheet demonstrates scaling payroll logic from weekly to monthly reporting.

---
## Files Included

- **Excel Workbook**
  - [Pay roll.xlsx](Pay%20roll.xlsx)

- **PDF Exports (Sheet-by-Sheet View)**
  - [Payroll Sheet (Base Pay)](payroll-sheet.pdf)
  - [Overtime & Bonus Sheet](overtime-bonus-sheet.pdf)
  - [January Payroll Sheet (Monthly Total)](january-payroll-sheet.pdf)

These PDFs allow reviewers to quickly understand the structure and calculations without opening Excel.


---

## Skills Demonstrated
- Microsoft Excel
- IF conditions
- SUM functions
- Payroll calculations
- Overtime and bonus logic
- Absolute and relative cell references
- Business data modeling
- Documentation and project presentation

---



