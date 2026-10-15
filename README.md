# 📊 Employee Attrition & Workforce Analytics Dashboard (Power BI)

##  Project Overview
This project presents an interactive executive Power BI dashboard designed to analyze workforce attrition across **1,470 employee records**. The objective is to identify key turnover drivers across department, demographic, and compensation metrics to assist HR leadership in developing data-driven retention strategies.

---

##  Key Business Findings
* **Department Breakdown:** Research & Development recorded the highest attrition count (**133 employees**), followed by Sales (**92 employees**).
* **Overtime Impact:** Employees working overtime experienced a **30.5% attrition rate**—nearly **3x higher** than non-overtime staff (**10.4%**).
* **High-Risk Roles:** **Sales Representatives** recorded the highest role-based turnover rate (**39.8%**), followed by Laboratory Technicians (**23.9%**).
* **Early-Career Turnover:** **36.4%** of overall attrition occurred within the **first year of tenure**, with the **18–25 age band** exhibiting the highest rate (**35.0%**).
* **Compensation Tiers:** Employees in the lowest salary tier (**<$5K/month**) represented **21.8%** of total turnover.
* **Gender Distribution:** Male employees accounted for **150 departures (63.3%)** vs. **87 departures (36.7%)** for Female employees.

---

##  Technical Stack & Implementation
* **Business Intelligence Tool:** Power BI Desktop
* **Data Transformation:** Power Query (Data cleaning, type casting, column formatting)
* **Data Modeling & DAX Measures:**
  * `Attrition Count` = `CALCULATE(COUNTROWS('WA_Fn-UseC_-HR-Employee-Attrition'), 'WA_Fn-UseC_-HR-Employee-Attrition'[Attrition] = "Yes")`
  * `Attrition Rate` = `[Attrition Count] / [Total Employees]`
  * `Average Monthly Income` = `AVERAGE('WA_Fn-UseC_-HR-Employee-Attrition'[MonthlyIncome])`
  * `Average Age` = `AVERAGE('WA_Fn-UseC_-HR-Employee-Attrition'[Age])`
* **UI/UX Design:** Standardized 3-tier grid layout, corporate navy/slate palette, high-contrast typography, locked visual containers, and interactive slicers.

---

##  Strategic Recommendations
1. **Early Onboarding & Mentorship:** Focus retention efforts on the first 1–2 years of employee tenure to reduce early drop-offs.
2. **Workload Rebalancing:** Implement overtime capping or additional compensation structures for high-demand roles like Sales Representatives and Lab Technicians.
3. **Compensation Benchmarking:** Review salary band thresholds for roles under $5K/month to align with industry benchmarks.

---

