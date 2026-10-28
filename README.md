# Budget vs Actual Finance Analysis (Excel)

An interactive Excel dashboard that measures how far actual spending ran over or under budget, by department, expense category and period.

## Business question
Where is the organisation overspending against budget, and which departments and expense categories drive the overruns?

## Dataset
- 10,000 unique transactions, Jan 2021 – Dec 2023 (10 duplicate rows removed during cleaning)
- Columns: Date, Department, Category, Region, Budget Amount, Actual Amount, Payment Method, Transaction ID
- 6 departments, 6 expense categories, 5 regions, 4 payment methods
- Synthetic sample data created for practice

## Tools
Excel: Pivot Tables, calculated field (% variance), Slicers, Timeline, charts

## Method
1. Cleaned the data: removed duplicate records and checked Transaction IDs are unique.
2. Added a calculated field: `% variance = (Actual − Budget) / Budget`.
3. Built pivot tables by department and by category.
4. Built a dashboard with charts, a Department/Category slicer and a date Timeline.

## Key findings
- Total spend ran **11.9% above budget**.
- **55.9%** of transactions were over budget.
- Biggest overruns by category: **Salaries (16.2%)**, then Utilities (12.6%) and Marketing (12.5%).
- Biggest overruns by department: **Marketing (15.1%)**, then HR (13.1%) and Sales (12.3%).
- Smallest overrun: Finance department (8.4%).

## Dashboard
<img width="1857" height="627" alt="image" src="https://github.com/user-attachments/assets/da625eea-9c09-4266-86be-b2405de89b29" />


## Files
```
data/        raw and cleaned data
workbook/    Budget_vs_Actual.xlsx
images/      dashboard screenshot
```

## Limitations
- Data is synthetic, so findings are illustrative, not real company results.
- Variance is measured on totals, not per transaction, because small budgets create extreme per-row percentages.

## Author
Ayush Kumar · [LinkedIn](https://www.linkedin.com/in/ayush-kumar-214742443) · ayushkum5591@gmail.com
