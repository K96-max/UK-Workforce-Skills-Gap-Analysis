# UK Workforce Skills Gap Analysis

A workforce insights project using the **UK Employer Skills Survey 2024** to explore where skills shortages are concentrated across industries and English regions, and how employer training measures relate to reported skills gaps.

> **Business context:** Employers need to understand where skills shortages are most acute so that workforce planning, recruitment, training and development investment can be directed towards the areas of greatest need.

## Business problem

Which industries and regions face the greatest skills-shortage pressures, and what does the available evidence suggest about the relationship between training and workplace skills gaps?

## Project objectives

- Compare the scale and concentration of skills gaps across industries.
- Identify regional differences in skill-shortage vacancies.
- Explore the relationship between training participation and skills-gap density.
- Translate the evidence into questions for workforce planning and learning investment.

## Data and approach

| | |
|---|---|
| Source | UK Employer Skills Survey 2024 |
| Original file | `core_indicators_11_24.csv` |
| Coverage | 13 industries and 9 English regions |
| Tools | Python, Pandas, Matplotlib, Jupyter Notebook and Tableau Desktop |
| Themes | Skills shortages, workforce capability and training |

1. **Data preparation:** inspected fields and data types, converted relevant measures to numeric formats, checked duplicates and treated unavailable survey codes as missing rather than zero.
2. **Industry analysis:** compared estimated skills-gap volumes, skills-gap density and the share of vacancies caused by skills shortages.
3. **Regional analysis:** compared skill-shortage vacancy measures across nine English regions and prepared regional results for mapping.
4. **Training analysis:** compared training participation with skills-gap density and calculated a Pearson correlation across the industry-level observations.
5. **Communication:** prepared analysis outputs for visual reporting. The Tableau dashboard and map remain in development and are not included in this repository yet.

## Key findings

### Industry

- **Wholesale & Retail** had the largest estimated employee skills-gap volume: **230,600**.
- **Hotels & Restaurants** had the highest skills-gap density: approximately **6.16%**.
- **Construction** had the highest proportion of vacancies caused by skills shortages: **45.02%**.
- **Public Administration** had the lowest proportion among the industries analysed: **6.65%**.

### Region

- The **South West** had the highest proportion of skill-shortage vacancies: **40.09%**.
- The **East of England** had the lowest proportion: **18.94%**.
- **London** had the highest estimated volume of skill-shortage vacancies: **45,600**.

### Training

Training participation and skills-gap density showed a **weak negative correlation (-0.17)** across the 13 industry-level observations analysed. This is not evidence that training directly reduces skills gaps.

## Business implications

The analysis suggests that a single national response may not address every skills challenge:

- Prioritise further investigation in industries with high skills-gap density and/or large shortage volumes.
- Consider regional labour-market conditions when planning workforce development.
- Evaluate training through capability and performance outcomes, not participation alone.
- Combine survey evidence with employer-level skills assessments, vacancy data and training outcomes before committing investment.

## Limitations

- The analysis is a snapshot of 2024 survey data, not a longitudinal evaluation.
- The training correlation is based on only 13 industry-level observations.
- Correlation does not establish causation.
- Regional comparisons cover the nine English regions, not every UK nation.
- Survey estimates and unavailable values must be interpreted in line with the source definitions.
- The Tableau workbook/dashboard and preview image are not yet included in this repository.
- The original `core_indicators_11_24.csv` source dataset is not included; users will need the source file locally to rerun the notebook.

## Repository contents

| Path | Contents |
|---|---|
| `Python/UK_Workforce_Skills_Gap_Analysis.ipynb` | Python analysis notebook |
| `Data/industry_analysis_2024.csv` | Industry-level analysis |
| `Data/regional_analysis_2024.csv` | Regional analysis |
| `Data/training_analysis_2024.csv` | Training analysis |

- [Python analysis](Python/UK_Workforce_Skills_Gap_Analysis.ipynb)
- [Prepared datasets](Data/)
- [Prepared data dictionary](Data/DATA_DICTIONARY.md)

## Business value

This project demonstrates how public workforce data can support skills planning: identifying where shortages are concentrated, comparing different measures of pressure, and assessing what further evidence is needed before recommending training or other interventions.

**Skills:** workforce analytics · data quality · missing-value handling · Pandas · exploratory analysis · correlation · regional analysis · visualisation · insight communication

---
*Portfolio project by K96-max.*
