# NHS HES Admission Outcomes Analysis

## Overview
This project analyses publicly available NHS Hospital Episode Statistics (HES) Admitted Patient Care data to explore variation in hospital length of stay across ethnic categories and its relationship with admission type.

The analysis uses aggregate population-level data and is intended as a descriptive exploration of healthcare utilisation patterns rather than a causal investigation.

## Data
The data were obtained from NHS England and consist of aggregated Admitted Patient Care activity tables for the 2024–2025 financial year. No individual-level or identifiable patient data were used.

## Methods
Data were imported into Python and cleaned to remove non-data header rows and empty columns. Ethnic category codes were retained alongside their descriptive labels for interpretability. Summary measures including mean and median length of stay, mean age, and counts of emergency and elective admissions were extracted.

An emergency admission proportion was calculated as the number of emergency admissions divided by the total number of emergency and elective admissions. Descriptive statistics and visualisations were used to examine variation across ethnic categories.

## Results
Mean length of stay varied across ethnic categories, ranging from approximately three to six days. Median length of stay was consistently low across groups, indicating that longer admissions were driven by a smaller proportion of episodes. Emergency admissions accounted for the majority of hospital activity across all ethnic categories, and a higher proportion of emergency admissions was associated with longer average hospital stays.

## Outputs
- Jupyter Notebook containing full analysis: `notebooks/01_hes_analysis.ipynb`
- Figures:
  - Mean length of stay by ethnic category
  - Emergency admission proportion vs mean length of stay

## Limitations
The analysis is based on aggregated administrative data and does not account for individual-level clinical, socioeconomic, or comorbidity factors. Findings describe population-level patterns and should not be interpreted as causal.

## Tools
- Python
- pandas
- matplotlib
- seaborn
