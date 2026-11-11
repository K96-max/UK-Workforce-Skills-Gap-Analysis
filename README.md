# UK Workforce Skills Gap Analysis

A workforce insights project using the **UK Employer Skills Survey 2024** to explore skills shortages across industries and English regions, and examine how employer training measures relate to reported skills gaps.

The project demonstrates how public workforce data can be cleaned, analysed and communicated to support evidence-informed people and workforce planning.

## Project at a glance

| | |
|---|---|
| Source | UK Employer Skills Survey 2024 |
| Original file | `core_indicators_11_24.csv` |
| Analysis | Python, Pandas, Matplotlib, Jupyter Notebook |
| Visualisation | Tableau Desktop |
| Coverage | 13 industries and 9 English regions |
| Themes | Skills shortages, workforce capability and training |

## Business questions

1. Which industries have the largest estimated employee skills-gap volumes?
2. Which industries and English regions have the highest proportions of skill-shortage vacancies?
3. What relationship can be observed between employee training participation and workplace skills gaps?

## Methodology

### 1. Data preparation
- Loaded and inspected the survey data in Python.
- Reviewed column types and converted relevant measures to numeric formats.
- Checked for duplicate records.
- Treated unavailable survey codes as missing values rather than zero.
- Distinguished national-level records from regional records where regional fields were structurally unavailable.

### 2. Industry analysis
Compared estimated skills-gap volumes, skills-gap density and the proportion of vacancies caused by skills shortages across 13 industries.

### 3. Regional analysis
Compared skill-shortage vacancy measures across nine English regions and prepared regional results for geographic visualisation.

### 4. Training analysis
Compared training participation with skills-gap density across industries and calculated a Pearson correlation to describe the direction and strength of the relationship.

### 5. Visualisation
Used Python for exploratory charts and Tableau Desktop for dashboard and geographic-map development.

## Key findings

### Industry patterns
- **Wholesale & Retail** had the largest estimated employee skills-gap volume: **230,600**.
- **Hotels & Restaurants** had the highest skills-gap density: approximately **6.16%**.
- **Construction** had the highest proportion of vacancies caused by skills shortages: **45.02%**.
- **Public Administration** had the lowest proportion of skill-shortage vacancies among the industries analysed: **6.65%**.

### Regional patterns
- The **South West** had the highest proportion of skill-shortage vacancies: **40.09%**.
- The **East of England** had the lowest proportion: **18.94%**.
- **London** had the highest estimated volume of skill-shortage vacancies: **45,600**.

### Training and skills gaps
Training participation and skills-gap density showed a **weak negative correlation (-0.17)** across the 13 industry-level observations analysed.

This is a weak association, not evidence that training directly reduces skills gaps. The small number of industry-level observations and the cross-sectional nature of the data limit the conclusions that can be drawn.

## Workforce implications

The findings suggest that workforce development should be targeted to the nature of the challenge:

- Consider skills development and progression pathways in industries with high skills-gap density.
- Combine vacancy-volume and vacancy-proportion measures when prioritising workforce interventions.
- Evaluate training using outcome measures, rather than assuming participation alone closes skills gaps.
- Investigate differences between regions and industries before designing interventions.

## Repository contents

| Path | Contents |
|---|---|
| `Python/UK_Workforce_Skills_Gap_Analysis` | Python notebook file |
| `Data/industry_analysis_2024.csv` | Industry-level analysis |
| `Data/regional_analysis_2024.csv` | Regional analysis |
| `Data/training_analysis_2024.csv` | Training analysis |

- [Open the Python analysis notebook](Python/UK_Workforce_Skills_Gap_Analysis.ipynb) · [Browse the Python folder](Python/)
- [Explore the prepared datasets](Data/)

## Limitations

- The analysis uses 2024 survey data and is a snapshot, not a longitudinal evaluation.
- The training correlation is based on 13 industry-level observations.
- Correlation does not establish causation.
- Regional comparisons cover the nine English regions, not every UK nation.
- Survey estimates and unavailable values should be interpreted in line with the source data.
- The Tableau dashboard and workbook are not currently present in the repository; these should be added with a dashboard preview before the project is presented as a finished visualisation case study.

## What this project demonstrates

**Workforce analytics · public-sector data · data quality assessment · missing-value handling · Pandas · exploratory analysis · correlation interpretation · regional analysis · data visualisation · communicating workforce insights**

---
*Portfolio project by K96-max.*
