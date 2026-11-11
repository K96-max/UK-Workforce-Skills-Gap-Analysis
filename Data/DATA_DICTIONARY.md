# Data dictionary – UK Employer Skills Survey 2024 outputs

These definitions describe the three prepared CSV files in this folder. Counts are estimates from the survey output; percentage measures are recorded as percentage values (for example, `40.09` means 40.09%, not 0.4009).

## `industry_analysis_2024.csv`

| Column | Meaning |
|---|---|
| `sector` | Industry sector used to group the national 2024 results |
| `skillgaps` | Estimated number of employees with skills gaps in the sector |
| `skillgap_inc` | Skills-gap incidence measure supplied by the source, expressed as a percentage |
| `skillgap_den` | Skills-gap density measure supplied by the source, expressed as a percentage |

## `regional_analysis_2024.csv`

| Column | Meaning |
|---|---|
| `region_name` | English region |
| `vac_sum` | Estimated total number of vacancies |
| `htfv_sum` | Estimated number of hard-to-fill vacancies |
| `ssv_sum` | Estimated number of skill-shortage vacancies |
| `ssv_percentage` | Calculated share of vacancies that are skill-shortage vacancies: `ssv_sum / vac_sum × 100` |

## `training_analysis_2024.csv`

| Column | Meaning |
|---|---|
| `sector` | Industry sector |
| `skillgaps` | Estimated number of employees with skills gaps |
| `skillgap_den` | Skills-gap density measure, expressed as a percentage |
| `training_den` | Training participation measure supplied by the source, expressed as a percentage |
| `train_days_employee` | Average training days per employee, as supplied by the source |
| `train_days_trainee` | Average training days per trainee, as supplied by the source |

## Interpretation and quality notes

- The outputs contain 13 industry records and 9 English-region records.
- The industry-level training comparison uses 13 observations. Its correlation is descriptive and does not establish that training causes skills gaps to rise or fall.
- The source dataset uses unavailable or unreliable-value codes (including `u`). These were converted to missing values during preparation rather than treated as zero.
- Check the original UK Employer Skills Survey 2024 technical documentation/codebook for the full denominator and calculation rules for each source measure before reusing the figures in formal reporting.
- These are derived analysis outputs, not the complete source dataset.
