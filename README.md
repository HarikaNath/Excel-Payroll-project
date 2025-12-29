# Excel Payroll Project (Hours, Overtime, Bonus, Monthly Total)

## Overview
This project is an Excel-based payroll calculator that:
- Computes weekly pay from hourly wage and hours worked
- Calculates overtime hours (hours over 40)
- Applies an overtime bonus (0.5 × hourly wage × overtime hours)
- Produces weekly total pay and a January month total per employee

## File
- `data/1st exercise Pay roll.xlsx`

---

## Sheet 1 — Payroll
**Purpose:** Calculate pay using Hours Worked and Hourly Wage.

**Columns**
- Last Name, First Name, Hourly Wage, Hours Worked, Pay

**Key Formula**
- Pay (example row): `=C4*D4`

---

## Sheet 2 — Overtime=Bonus
**Purpose:** Add overtime logic + bonus + total pay.

**Key Formulas**
- Overtime Hours: `=IF(D8>40,D8-40,0)`
- Pay: `=C8*D8`
- Overtime Bonus: `=0.5*C8*E8`
- Total Pay: `=F8+G8`

---

## Sheet 3 — Jan Payroll
**Purpose:** Extend payroll across multiple January weeks and compute monthly totals.

### Weekly structure
- Hours Worked: `D:H`
- Overtime Hours: `I:M`
- Pay: `N:R` using absolute hourly wage references (example `=$C4*D4`)
- Overtime Bonus: `S:W` (example `=0.5*$C4*I4`)
- Total Pay: `X:AB` (example `=N4+S4`)
- Jan Pay (Monthly Total): `AD` (example `=SUM(X4:AB4)`)

---

## Skills Demonstrated
- Excel formulas: IF, SUM, arithmetic operations
- Absolute references ($C4) for consistent wage calculations
- Payroll logic modeling (weekly → monthly rollup)

## Screenshots
See `docs/screenshots/`
