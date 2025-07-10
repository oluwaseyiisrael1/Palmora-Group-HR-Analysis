# Palmora-Group-HR-Analysis
Power BI–based Human Resources analysis for Palmora Group to uncover gender inequality, salary distribution, pay gaps, and bonus allocation insights.

# 📊 Palmoria Group – HR Analytics Report (Power BI)

## 👔 Project Overview

This Power BI dashboard was developed to help Palmoria Group identify and address gender inequality and pay equity issues within its workforce across different regions and departments. In addition to analyzing employee demographics, ratings, and salaries, we also calculated performance-based bonuses for each employee using external bonus rules.

---

## 📁 Data Sources
- `Palmoria Group emp-data.csv` – Core HR dataset
- `BonusRules.xlsx` – Bonus percentage rules based on performance ratings

---

## 🧩 Key Data Cleaning Steps
- Removed employees with missing or `NULL` departments
- Removed records with blank or zero salaries
- Standardized undefined gender entries as `Unidentified`
- Mapped text-based performance ratings to numeric scores for analysis
- Applied performance-based bonus percentages using a lookup

---

## 📌 Key Insights & Visuals

### 1. Gender Distribution by Department and Region
- **Visuals**: Stacked Bar + Matrix
- Insight: Male employees dominate most departments. Some departments and regions have low or no female representation, suggesting gender imbalance in recruitment or retention.

---

### 2. Average Performance Rating by Gender
- **Visual**: Clustered Column Chart (using mapped rating scores)
- Insight: While average ratings are close, females slightly outperform males in some departments. However, rating distribution is fairly balanced overall.

---

### 3. Gender Pay Gap Analysis
- **Visuals**: Matrix & Clustered Column Chart by Region/Department
- Insight:
  - Overall, males earn slightly more than females across regions.
  - Significant disparities observed in specific departments like Sales and Engineering in the Northern region.
  - Management should audit salary structure in these departments.

---

### 4. Salary Regulation Compliance & Pay Distribution
- **Requirement**: Employees must earn a minimum of **$90,000**
- **Visuals**:
  - Histogram (Salary Bands in $10K increments)
  - Region-wise Salary Distribution
  - Card showing % of employees below $90K
- Insight:
  - ~69% of employees earn **below $90,000**
  - Most of these employees are clustered in non-technical roles across regions
  - Company may need a compensation review to meet regulatory standards

---

## 💸 Bonus Allocation Insights

**Data Source**: `BonusRules` file mapped to employee ratings

### 🎯 Calculated Columns:
- `BonusRate` – percentage lookup from BonusRules
- `BonusAmount` – calculated from BonusRate × Salary
- `TotalPayWithBonus` – Salary + BonusAmount

### 🔍 Visuals:
- **Matrix**: Shows Name, Salary, Bonus Rate, Bonus Amount, Total Pay
- **Cards**:
  - Total Bonus Paid
  - Total Compensation Paid (Salary + Bonus)
- **Bar Chart**: Bonus Allocation by Region

**Insight**:
- The total company-wide bonus paid is well distributed by region.
- Management can use this for annual planning and workforce cost estimation.

---

## ✅ Recommendations
- Increase female representation in underrepresented departments
- Review salary structures in Sales, Engineering, and Logistics
- Adjust compensation to align with the $90K minimum rule
- Continue using transparent bonus allocation frameworks based on performance

---

## 🔗 Tools Used
- Microsoft Power BI Desktop
- DAX for measures and columns
- Power BI Modeling for data relationships

---

## ✍️ Prepared by:
Oluwaseyi Israel (HR Analytics Consultant) For DSA Data Analysis Final Project
🔗 [LinkedIn] https://linkedin.com/in/oluwaseyi-israel/
🔗 https://github.com/oluwaseyiisrael1/Palmora-Group-HR-Analysis
