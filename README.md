# UK-Workforce-Skills-Gap-Analysis
Analysis of UK workforce skills shortages, regional differences and employer training using Python and Tableau.

# UK Workforce Skills Gap Analysis (2024)

## Project Overview

This project analyses the UK Employer Skills Survey 2024 to investigate skills shortages across UK industries and English regions, and explore the relationship between employee training and workplace skills gaps.

The aim was to identify where skills shortages are most significant and consider how employers can use workforce development and training to address changing skills requirements.

## Business Questions

The analysis focuses on three key questions:

1. Which UK industries experience the largest workforce skills gaps?
2. Which English regions have the highest proportions of skill-shortage vacancies?
3. Is there an observable relationship between employee training participation and workplace skills gaps?

## Tools and Technologies

- **Python:** Data cleaning, preparation, exploratory data analysis and visualisation.
- **Pandas:** Data manipulation, filtering, aggregation and analysis.
- **Matplotlib:** Data visualisation.
- **Tableau Desktop:** Interactive dashboard development and geographic mapping.
- **Jupyter Notebook:** Analysis documentation and reproducible code.

## Data Source

UK Government – Employer Skills Survey 2024.

Original dataset: `core_indicators_11_24.csv`

The dataset contains information on vacancies, hard-to-fill vacancies, skill-shortage vacancies, employee skills gaps and employer-funded training.

## Methodology

### 1. Data preparation
- Imported the original survey dataset into Python.
- Inspected the dataset structure, columns and data types.
- Converted relevant numerical fields into appropriate numeric formats.
- Identified unavailable values and preserved them as missing rather than treating them as zero.
- Investigated missing values and confirmed that regional fields were structurally unavailable for national-level records.
- Checked for duplicate records.

### 2. Industry analysis
Compared estimated employee skills-gap volumes, skills-gap density and the proportion of vacancies caused by skills shortages across 13 industries.

### 3. Regional analysis
Compared skill-shortage vacancy volumes and proportions across nine English regions. Joined the regional analysis to official ONS geographic boundary data to create a Tableau map.

### 4. Training analysis
Compared employee training participation with skills-gap density across 13 industries. Used correlation analysis to explore the strength and direction of the relationship.

### 5. Dashboard development
Created a Tableau dashboard combining industry comparisons, regional mapping, training analysis and key performance indicators.

## Key Findings

### Industry skills gaps
- Wholesale & Retail had the largest estimated employee skills-gap volume, at **230,600**.
- Hotels & Restaurants had the highest skills-gap density, at approximately **6.16%**.
- Construction had the highest proportion of skill-shortage vacancies, at **45.02%**.

### Regional skills shortages
- The South West had the highest proportion of skill-shortage vacancies, at **40.09%**.
- The East of England had the lowest proportion, at **18.94%**.
- London had the highest estimated volume of skill-shortage vacancies, at **45,600**.

### Training and skills gaps
- Training participation and skills-gap density showed a weak negative correlation of **-0.17** across the 13 industries analysed.
- This indicates a weak association, not evidence that increased training directly reduces skills gaps.
- Training participation and training intensity varied considerably between industries.

## Business Implications

The findings suggest that employers should consider both the volume and proportion of skills shortages when planning workforce development.

Industries with high skills-gap density may benefit from targeted training and development programmes, while sectors with high vacancy volumes may require broader workforce planning and recruitment strategies.

Understanding the relationship between training investment and skills gaps can help organisations make more informed decisions about their people strategies.

## Limitations

- The analysis uses 2024 survey data and provides a snapshot rather than a longitudinal assessment of training effectiveness.
- The training correlation is based on 13 industry-level observations.
- Correlation does not establish causation.
- Regional comparisons cover England's nine regions, rather than the whole of the UK.
- Survey estimates and unavailable values should be interpreted in line with the source data.

## Project Files

- `Data/` – Cleaned industry, regional and training analysis datasets.
- `Python/` – Jupyter Notebook containing the data preparation and analysis.
- `Tableau/` – Packaged Tableau workbook and dashboard image.
- `README.md` – Project documentation.

## Conclusion

This project demonstrates how workforce survey data can be transformed into meaningful insights using Python and Tableau.

It combines data preparation, exploratory analysis, statistical interpretation and visual storytelling to investigate UK workforce skills shortages and employer training activity.
