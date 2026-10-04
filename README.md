# HR Recruitment Analytics

An Excel-based HR analytics project that examines which factors are linked to hiring decisions across 200,000 candidates, presented in an interactive dashboard with recommendations for HR.

## Dashboard

![Dashboard](images/dashboard.png)

## Objective

Identify which candidate attributes (experience, internships, skills, education, university tier, and company type) are most closely related to the chance of being hired, so HR can make screening more focused.

## Dataset

- 200,000 candidates with 17 original columns (age, education level, university tier, CGPA, internships, projects, skills, experience, hiring outcome, etc.)
- 4 columns added during cleaning, including a `Data_Flag` column that marks invalid rows
- 195,871 valid candidates were analyzed (overall hire rate: 70.4%)
- 4,129 rows were excluded: 181 rows with CGPA above 10 and 3,948 rows where years of experience exceeded working age
- ⚠️ The data appears to be **synthetic (dummy data)**, so the results are illustrative and do not describe any real company.

## Process

1. **Data cleaning:** converted numbers stored as text, flagged invalid rows, and excluded them from the analysis
2. **Grouping:** created bands for experience (<1, 1-3, 3-5, 5+ years) and skills score
3. **Analysis:** built PivotTables for hire rate by each factor
4. **Dashboard:** KPI cards, PivotCharts, and slicers for interactive filtering
5. **Insights:** summarized findings with supporting numbers and recommendations

## Insights & Recommendations

![Insights](images/insight.png)

## Key Findings

| # | Finding | Evidence | Recommendation |
|---|---------|----------|----------------|
| 1 | Work experience is most strongly linked to being hired | Hire rate rises from 68.1% (<1 year) to 81.5% (5+ years), a 13.4-point gap | Give more weight to relevant experience when screening CVs |
| 2 | Internship experience is linked to a higher hire rate | Hire rate rises from 67.8% (0 internships) to 81.3% (7 internships), a 13.5-point gap | Prioritize candidates with internship history, especially for entry-level roles |
| 3 | A high skills score is linked to a higher hire rate, but the effect is smaller | Hire rate rises from 67.7% (score ≤10) to 74.0% (score >20), a 6.3-point gap | Use skills score as supporting input, not the sole deciding factor |
| 4 | Education level, university tier, and company type barely differ | Education 70.3-70.6%, university tier 70.4-70.5%, company type 70.3-70.6% | Reduce reliance on degrees and campus name as early filters |

## Limitations

- The data is synthetic (flat patterns across many variables), so results may differ from real company data.
- The relationships found are correlations, not cause and effect.
- Candidates with 8 or more internships (at most 24 people) were not analyzed because the sample is too small.

## Workbook Structure

| Sheet | Content |
|-------|---------|
| Cover | Project overview and table of contents |
| Dashboard | KPIs and interactive charts with slicers |
| Insight | Findings, evidence, and recommendations |
| Analysis | PivotTables per factor |
| Chart_Data | Source pivots for the charts |
| Clean_Data | Cleaned data with validity flags |

## Tools

Microsoft Excel: PivotTable, PivotChart, Slicer, formulas

## How to Open

[Download HR_Recruitment_Analytics.xlsb](https://github.com/Aulia-Akbar/hr-recruitment-analytics/raw/main/HR_Recruitment_Analytics.xlsb) and open it in Microsoft Excel. The file uses the Excel Binary format (.xlsb) to stay under GitHub's file size limit. If the dashboard looks empty, click **Data > Refresh All**.

## Author

**Hikmal Aulia Akbar**
[LinkedIn](https://www.linkedin.com/in/hikmal-aulia-akbar-a31373314) · [Email](mailto:hikmalgood56@gmail.com)
