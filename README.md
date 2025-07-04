# Palmoria Group HR Analytics Dashboard (Power BI)

## Overview  
Palmoria Group is a manufacturing company dealing with HR issues related to gender imbalance, performance gaps, and salary inequality across regions and departments. The company needed a detailed analysis to uncover these issues and take corrective actions.

This project involved analyzing employee data using Power BI. I cleaned and prepared the data, built relationships between tables, and created a multi-page dashboard to help management understand patterns in gender distribution, performance, salary structure, and bonus allocation.

## Tools Used  
- Power BI Desktop  
- Power Query  
- Data Modeling (Relationships, Measures, DAX)  
- Custom Columns and Calculated Fields  
- Stacked Bar Charts, Pie Charts, and KPI Cards

## Objective  
To help Palmoria’s management team identify HR challenges like gender imbalance, pay gaps, and compliance with salary regulations. The final deliverable was a 4-page interactive Power BI dashboard with charts, metrics, and filters.

## Key Steps

### 1. Data Cleaning  
- Removed employees without salary (former staff)  
- Removed rows with NULL departments  
- Handled missing or undisclosed gender values  
- Converted performance ratings from text to numeric values  
- Created additional fields like Salary Bands and Join Keys for lookup 

### 2. Data Modeling  
- Built relationships between the main employee table and a bonus rules table  
- Used a custom `JoinKey` (Department + Rating) to match bonus rules  
- Created calculated columns using DAX for Bonus Amount and Total Pay  
![Image](https://github.com/user-attachments/assets/030cce4a-0f33-4a7a-bf4d-f68b180ecd47)

### 3. Dashboard Development (4 Pages)
[DSA Data analysis Power BI.pdf](https://github.com/user-attachments/files/21068784/DSA.Data.analysis.Power.BI.pdf)

#### Page 1: Gender Overview  
- Overall gender distribution  
- Gender breakdown by department and region  
- Employee count summary

#### Page 2: Performance & Ratings  
- Rating distribution by gender  
- Average rating per department  
- Optional slicers for filtering by region or department

#### Page 3: Salary Insights  
- Salary band distribution (grouped by $10K)  
- Salary band by region  
- Average salary by gender (company-wide, by region, and by department)  
- Compliance check for $90K minimum wage (KPI card and employee count)

#### Page 4: Bonus Allocation  
- Bonus amount by region  
- Total bonus payout card (company-wide)  
- Total pay (salary + bonus) chart  
- Optional slicers by department or rating
[Gender.pdf](https://github.com/user-attachments/files/21068889/Gender.pdf)
[Bonus Allocation.pdf](https://github.com/user-attachments/files/21068886/Bonus.Allocation.pdf)
[Salary Regulation.pdf](https://github.com/user-attachments/files/21068887/Salary.Regulation.pdf)
[Salary structure.pdf](https://github.com/user-attachments/files/21068888/Salary.structure.pdf)


## Key Measures and Calculations  
- **Bonus Amount** = Bonus % × Salary  
- **Total Pay** = Salary + Bonus  
- **Employees Below 90K** = Count of employees earning less than regulation threshold  
- **Salary Band** = Grouping by $10K ranges for visual distribution  

## Questions Answered

**Q1. What is the gender distribution across the organization, departments, and regions?**  
Answer: Visualized using pie and stacked bar charts on Page 1.
[Gender.pdf](https://github.com/user-attachments/files/21068889/Gender.pdf)

**Q2. How do performance ratings differ by gender?**  
Answer: Page 2 shows rating averages per gender.
[Salary structure.pdf](https://github.com/user-attachments/files/21068888/Salary.structure.pdf)

**Q3. Is there a gender-based salary gap? If yes, where?**  
Answer: Found in the salary visuals on Page 3, broken down by region and department.
[Salary Regulation.pdf](https://github.com/user-attachments/files/21068887/Salary.Regulation.pdf)

**Q4. Are salaries compliant with the $90,000 minimum regulation?**  
Answer: Yes/No (based on result). The dashboard displays count of employees below $90K and the distribution by region.

**Q5. How are bonuses allocated, and what is the total payout?**  
Answer: Page 4 shows total bonuses, per region, and per employee.
[Bonus Allocation.pdf](https://github.com/user-attachments/files/21068886/Bonus.Allocation.pdf)

## What I Learned  
This project taught me how to take raw HR data and turn it into interactive business insights using Power BI. I practiced advanced Power Query transformations, DAX formulas, and dashboard design across multiple pages. I also learned how to model relationships between tables and deal with real-world data challenges like duplicates, NULLs, and missing joins.
