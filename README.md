# HR Attrition Dashboard (Excel)

An interactive Excel dashboard analysing employee attrition in the IBM HR Analytics dataset (1,470 employees). It shows where attrition is highest and which areas HR should look at first.

![HR Attrition Dashboard](images/dashboard.png)

## Project Overview

**Business question:** Which groups of employees are leaving the most, and where should HR focus retention efforts?

**Headline result:** 237 of 1,470 employees left (**16.12% attrition**). Attrition is concentrated in specific groups, especially employees working overtime, early-tenure employees, and the lowest salary band.

## Dataset

- **Source:** IBM HR Analytics Employee Attrition & Performance dataset (a fictional dataset created by IBM data scientists)
- **Size:** 1,470 employees, 35 original columns
- **Columns added by me:** `Attrition Flag` (1/0), `Salary Band` (income quartiles), tenure bands and age bands

## Key Findings

| Area | Finding |
|---|---|
| **Overall** | 237 leavers out of 1,470 (16.12%) |
| **Department** | Sales is highest at 20.63%, then HR (19.05%) and R&D (13.84%) |
| **Overtime** | 30.53% attrition with overtime vs 10.44% without, about 2.9x higher |
| **Sales + overtime** | 37.5% attrition, and this group accounts for about 20% of all exits |
| **Tenure** | 0-4 years of service is highest at 24.31%; 15-20 years is lowest at 6.52% |
| **Salary** | Lowest income quartile 29.27% vs 10.33% in the highest, about 2.8x |
| **Job satisfaction** | Rating 1 had 22.84% attrition vs 11.33% for rating 4 |
| **Job role** | Sales Representatives are highest at 39.76% |
| **Age** | Under-25s are highest at 39.18% |
| **Marital status** | Single employees 25.53%, vs 12.48% married and 10.09% divorced |
| **Gender** | Small gap: 17.01% male vs 14.80% female |

## Recommendations

1. **Review overtime and workload in Sales.** Sales employees working overtime left at 37.5%, against 13.8% for those who didn't. Check sales targets, overtime compensation and rest.
2. **Strengthen onboarding and early-tenure support.** Add structured check-ins in the first 1-2 years and clearer manager support.
3. **Review pay and progression for the lowest salary band.** Look at salary competitiveness, promotion paths and raises.
4. **Monitor job satisfaction.** Use pulse surveys to catch problems early.
5. **Pilot retention actions with Sales Representatives**, the role with the highest attrition.

## Dashboard Features

- KPI cards: total employees, employees left, attrition rate, retention rate, overtime attrition, early-tenure attrition
- 11 charts covering department, overtime, job role, tenure, salary band, job satisfaction, age, gender, marital status, and department x overtime
- Interactive slicers: Department, Job Role, Gender, Marital Status, Overtime Status
- Key Insights panel and a Recommendations section

## Tools & Skills

- **Microsoft Excel:** PivotTables, PivotCharts, slicers, Excel Tables, structured references, `GETPIVOTDATA`, formulas
- **Data preparation:** calculated columns (flags, bands), data checks
- **Analysis:** segmentation, rate comparisons, identifying overlapping risk groups
- **Dashboard design:** KPI cards, chart layout, formatting, consistent colours
- **Communication:** turning findings into HR recommendations

## Limitations

- These are **associations, not proven causes**. For example, overtime is linked to higher attrition, but this analysis doesn't show that overtime causes people to leave.
- The high-attrition groups (overtime, low salary, early tenure) **may overlap**. I compared them separately and didn't test whether the same employees fall in each.
- Some segments are small. For example, Sales Representatives are only 83 employees, so their rate should be read with caution.
- The IBM dataset is fictional, so the results illustrate the method rather than describe a real company.

## Next Steps

- Check how overtime, salary band and tenure interact, for example overtime attrition within each salary band
- Add a statistical test or regression to see which factors matter most
- Rebuild the dashboard in Power BI or Tableau

## Files

- `HR_Attrition_Dashboard.xlsx`: the full workbook (data, pivots, dashboard)
- `images/dashboard.png`: dashboard screenshot

## Author

**[Your Name]**: [LinkedIn link] | [Portfolio link]
