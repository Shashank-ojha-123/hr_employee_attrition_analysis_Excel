# 👥 HR Employee Attrition Analysis
### Microsoft Excel | Pivot Tables | Dashboard | DAX

---

## 📊 Dashboard Overview
![Dashboard](/screenshot/dashboard_overview.PNG)

---

## 📌 About This Project
Analyzed IBM HR Analytics dataset of 1,470 employees
to identify key drivers of employee attrition and
provide actionable retention recommendations for HR
decision makers. Built entirely in Microsoft Excel
using advanced formulas, pivot tables, and an
interactive dashboard.

| Detail | Info |
|---|---|
| Dataset | IBM HR Analytics Employee Attrition (Kaggle) |
| Tool | Microsoft Excel 2019 |
| Dataset Size | 1,470 employees, 35 variables |
| Overall Attrition Rate | 16.12% |
| Total Attrited Employees | 237 |
| Average Monthly Salary | ₹6,502.93 |

---

## ❓ Business Problems Solved

1. Which age group has the highest attrition rate
   and what is their average salary?
2. Do employees with long commutes have higher
   attrition rates than nearby employees?
3. Are experienced high performers leaving
   disproportionately?
4. Are low paid high performing employees leaving
   at higher rates?
5. Does job satisfaction predict attrition
   independently of salary?

---

## 🔍 Key Insights

**1. Young Employees Are Leaving Most**
Employees aged 18-30 have the highest attrition
rate at 25.91% — more than double the 46-60 age
group. With a ₹6,000 average salary gap between
youngest and oldest employees, insufficient
compensation progression for early career staff
is a likely contributing factor.

**2. Job Satisfaction is the Strongest 
Retention Predictor**
Employees with lowest job satisfaction leave at
22.84% versus just 11.33% for highly satisfied
employees — exactly double the rate. Critically
this difference exists despite similar salary
levels proving satisfaction predicts attrition
independently of pay.

**3. Long Commute Employees Leave Despite 
Higher Salaries**
Employees commuting 20+ km show the highest
attrition at 22.06% despite earning the highest
average salary among all distance groups.
Commute burden outweighs financial compensation
suggesting flexible or hybrid work arrangements
would be more effective than salary increases
for this segment.

**4. Rising Stars Are Leaving Early**
New high performers with under 10 years tenure
and rating 4 are leaving at 18.68% — the most
critical retention risk in the dataset. These
are the company's future leaders being lost
before reaching their potential. Meanwhile
experienced high performers with 20+ years
show zero attrition confirming the company
retains its best veterans but loses its
best newcomers.

**5. Good Performers Leave More Than 
Excellent Performers**
Rating 3 employees show higher overall attrition
than rating 4 employees suggesting the company
is retaining its absolute best talent while
losing mid tier performers — a pattern of
healthy attrition at the top but concerning
talent drain in the middle.

---

## 💡 Business Recommendations

1. **Review junior salary bands urgently**
   18-30 age group attrition at 25.91% combined
   with a ₹6,000 salary gap versus older employees
   suggests early career compensation is
   insufficient to retain young talent

2. **Invest in culture and satisfaction 
   over blanket salary increases**
   Job satisfaction predicts attrition independently
   of pay — HR investment in recognition, career
   development and work environment delivers
   better retention ROI than salary increases alone

3. **Introduce flexible work for long 
   commute employees**
   22.06% attrition among 20+ km employees despite
   highest salaries proves money cannot compensate
   for commute burden — hybrid or remote options
   would be more effective

4. **Fast track recognition for new 
   high performers**
   18.68% attrition among new excellent performers
   represents the highest value retention risk —
   accelerated promotion pathways and early
   recognition programs would protect this
   critical talent segment

5. **Investigate mid tier performer satisfaction**
   Rating 3 employees leaving at higher rates than
   rating 4 suggests a middle talent drain that
   could impact operational capacity over time

---

## 🛠️ Excel Skills Demonstrated

**Data Cleaning:**
- Removed redundant columns with zero analytical
  value (EmployeeCount, StandardHours, Over18)
- Converted table format for structured references
- Verified data integrity with COUNTBLANK

**Calculated Columns Using IFS Formula:**
- AttritionFlag — converted Yes/No to 1/0
- AgeGroup — 4 segments (18-30, 31-45, 46-60, 60+)
- SalaryBand — 4 bands (0-5k, 5k-10k, 10k-15k, 15k+)
- DistanceGroup — 3 segments (0-10, 11-20, 20+)
- TenureGroup — 4 segments (0-10, 10-20, 20-30, 30+)
- PerformanceGroup — converted 3/4 to Good/Excellent
- SatisfactionGroup — converted 1-4 to labels

**Pivot Table Analysis:**
- Multi dimensional analysis combining 2 variables
- Average of binary flag for attrition rate calculation
- Cross dimensional salary vs attrition comparison

**Dashboard:**
- 4 KPI cards with live formula references
- 4 interactive PivotCharts with data labels
- Conditional color coding — red for high attrition
- 3 connected slicers — Department, Gender,
  BusinessTravel
- All slicers connected to all pivot tables
  simultaneously via Report Connections

---

## 📊 Analysis Summary

| Business Question | Key Finding |
|---|---|
| Attrition by Age | 18-30 highest at 25.91% |
| Attrition by Commute | 20+ km highest at 22.06% |
| Performance vs Tenure | New high performers 18.68% |
| Satisfaction vs Salary | Low satisfaction 22.84% vs 11.33% |
| Overall Attrition | 16.12% across 1,470 employees |

---

## 📁 Repository Structure
```
HR-Attrition-Excel-Analysis/
│
├── README.md
│
├── HR_Attrition_Analysis.xlsx
│
├── screenshots/
│   ├── dashboard_overview.png
│   ├── pivot_age_attrition.png
│   ├── pivot_commute_attrition.png
│   ├── pivot_performance_tenure.png
│   └── pivot_satisfaction_attrition.png
│
└── data/
    └── source_link.md
```

---

## 📂 Data Source
Dataset sourced from Kaggle:
[IBM HR Analytics Employee Attrition Dataset]
(Source: https://www.kaggle.com/datasets/pavansubhasht/
)

Real IBM HR dataset used widely for people
analytics research and education.
Used for educational and portfolio purposes only.

---

## 📉 Methodology Notes

**Attrition Rate Calculation:**
AttritionFlag column (1=Left, 0=Stayed) was created
from Yes/No Attrition column. Average of this binary
flag in pivot tables automatically calculates
attrition rate per segment — same logic as
proportion calculation in SQL and DAX.

**Statistical Approach:**
All findings based on complete dataset of 1,470
employees with no sampling or exclusions — dataset
size sufficient for reliable segment level analysis
without minimum threshold filtering.
```
