# UK Labour Market Intelligence

A practical time-series analysis project using Office for National Statistics labour-market indicators. The work explores employment, unemployment, economic activity and inactivity across the UK over time.

## Dataset

- **File:** `Data/ons_uk_labour_market_clean.csv`
- **Records:** 666 rolling three-month observations
- **Period covered:** Jan–Mar 1971 to Jun–Aug 2026
- **Measures:** economic activity, employment, unemployment and economic inactivity rates
- **Age groups:** population aged 16+ and 16–64

The uploaded CSV is the cleaned analysis extract used in the MySQL workflow. It contains percentage measures and a period field.

## Questions explored

- How have UK employment and unemployment rates changed over time?
- How do the 16+ and 16–64 measures compare?
- How did labour-market conditions change during major economic periods?
- What do employment, unemployment and inactivity indicators reveal when considered together?

## Tools and learning

Python / Pandas for data inspection and preparation; MySQL for importing, querying and comparing time-series observations; Excel and Tableau for reporting and dashboard presentation.

## Current status

**Data preparation and MySQL practice:** documented.  
**SQL scripts:** available in the `SQL/` folder.  
**Dashboard:** to be added by the author.  
**Further work:** validate historical comparisons against ONS definitions and publish dashboard screenshots or a Tableau workbook.

## SQL files

- `SQL/01_Data_Exploration.sql` — table inspection, schema review, record count and data preview.
- `SQL/02_Financial_Crisis_Comparison.sql` — annual average employment and unemployment comparison for 1979–1987 and 2007–2015.

## Data quality and interpretation

ONS labour-market rates are published as rolling three-month estimates. Adjacent observations overlap, so they should not be treated as independent monthly observations. Interpret comparisons using the relevant ONS definitions and reference population.

---
*Portfolio learning project by K96-max.*
