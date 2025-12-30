# NHS Hospital Episode Statistics: Admission Outcomes by Ethnicity

## Overview

This project presents a descriptive analysis of publicly available **NHS Hospital Episode Statistics (HES)** Admitted Patient Care data, examining variation in hospital length of stay and admission type across ethnic categories in England.

Using aggregated, anonymised administrative data, the analysis focuses on **population-level patterns** rather than individual-level outcomes. The study provides insight into how admission pathways and demographic structure may be associated with hospital resource utilisation across different ethnic groups.

---

## Aim

The aim of this analysis was to:

- Examine differences in **mean length of hospital stay** across ethnic categories  
- Explore the relationship between **emergency admission proportion** and **length of stay** using aggregate NHS HES Admitted Patient Care data.

---

## Data Source

- **NHS Hospital Episode Statistics (HES)**  
- Admitted Patient Care (APC) activity tables  
- Reporting year: **2024–25**  
- Data accessed in **publicly available, aggregated format**

---

## Methods

- Retrospective observational analysis of aggregate HES data  
- Data imported, cleaned, and processed using **Python (pandas)**  
- Admissions grouped by **ethnic category**  
- Emergency admission proportion calculated as:  
  **Emergency admissions ÷ (Emergency + Elective admissions)**  
- Descriptive statistics used to summarise:
  - Mean length of stay  
  - Median length of stay  
  - Mean age  
  - Emergency admission proportion  
- Data visualisations produced using **matplotlib** and **seaborn**

---

## Key Results

### Mean Length of Stay by Ethnic Category

Figure 1 presents the top 15 ethnic categories ranked by mean length of hospital stay.

Mean length of stay varied across ethnic categories. **Irish (White)** and **Caribbean (Black or Black British)** groups exhibited higher average lengths of stay compared with other groups. These differences may reflect variation in **age structure**, **case mix**, and **admission pathways**, rather than ethnicity itself.


### Figure 1. Mean Length of Stay by Ethnic Category

The figure below shows the top 15 ethnic categories ranked by mean length of hospital stay.

![Mean length of stay by ethnic category](mean_los_by_ethnicity_top15.png)

---

### Emergency Admission Proportion and Length of Stay

Figure 2 illustrates the relationship between emergency admission proportion and mean length of stay.

A **positive association** was observed between higher emergency admission proportions and longer average hospital stays. Ethnic groups with a greater reliance on emergency admissions tended to experience increased mean length of stay. This pattern is consistent with the higher clinical complexity and acuity typically associated with emergency care.

### Figure 2. Emergency Admission Proportion vs Mean Length of Stay

This scatter plot illustrates the relationship between the proportion of emergency admissions and mean length of hospital stay across ethnic categories.

![Emergency admission proportion vs mean length of stay](emergency_prop_vs_mean_los.png)

---

### Summary Statistics

- Mean length of stay ranged approximately from **2.8 to 6.1 days** across ethnic categories  
- Emergency admissions accounted for a **high proportion (>95%)** of admissions in most groups  
- Mean age varied substantially between groups, which may partially explain observed differences in length of stay  

---

## Limitations

- Analysis is based on **aggregated data**, precluding individual-level inference  
- No adjustment for comorbidities, diagnosis, or socioeconomic factors  
- Observed associations are **descriptive rather than causal**

---

## Conclusion

This analysis demonstrates meaningful variation in hospital length of stay across ethnic categories within NHS Admitted Patient Care data. Groups with higher proportions of emergency admissions tended to experience longer average hospital stays, highlighting the importance of **admission pathway** and **demographic structure** when interpreting population-level hospital utilisation patterns.

The findings illustrate the value of routinely collected administrative data for health services research, while underscoring the need for cautious interpretation when individual-level clinical detail is unavailable.

---

## Tools Used

- Python  
- pandas  
- matplotlib  
- seaborn  
- Jupyter Notebook  

---

## Repository Contents

- `01_hes_analysis.ipynb` — Full analysis notebook  
- `mean_los_by_ethnicity_top15.png` — Figure 1: Mean length of stay by ethnic category  
- `emergency_prop_vs_mean_los.png` — Figure 2: Emergency admission proportion vs length of stay  
- `ethnicity_los_summary.csv` — Summary statistics table  


