**NHS Hospital Episode Statistics: Admission Outcomes by Ethnicity**
 
 **Overview**
This project presents a descriptive analysis of publicly available NHS Hospital Episode Statistics (HES) Admitted Patient Care data to explore variation in hospital length of stay and admission type across ethnic categories in England.

Using aggregated, anonymised data, the analysis focuses on population-level patterns rather than individual-level outcomes, providing insight into how admission pathways and demographic structure may relate to hospital resource utilisation.
  
   **Aim :**
To examine differences in mean length of hospital stay across ethnic categories and to explore the relationship between emergency admission proportion and length of stay using aggregate NHS HES data.
   
   **Data Source**
   
NHS Hospital Episode Statistics (HES)

Admitted Patient Care (APC) activity tables.

Reporting year: 2024–25

Data accessed in aggregated, publicly available format.

   **Methods**

Retrospective observational analysis of aggregate HES data

Data imported and cleaned using Python (pandas)

Admissions grouped by ethnic category

Emergency admission proportion calculated as:
Emergency admissions ÷ (Emergency + Elective admissions)

Descriptive statistics used to summarise:
Mean length of stay, Median length of stay, Mean age, Emergency admission proportion

Visualisations produced using matplotlib and seaborn

 **Key Results**

Mean Length of Stay by Ethnic Category

Figure 1 shows the top 15 ethnic categories ranked by mean length of hospital stay.

Mean length of stay varied across ethnic categories

Irish (White) and Caribbean (Black or Black British) groups showed higher average lengths of stay

Differences may reflect variation in age structure, case mix, and admission pathways

Emergency Admission Proportion vs Mean Length of Stay

The relationship between emergency admission proportion and mean length of stay is shown below.

A positive association was observed between higher emergency admission proportions and longer average hospital stays

Groups with a greater reliance on emergency admissions tended to have increased mean length of stay

This pattern is consistent with higher clinical complexity typically associated with emergency care
 
 **Summary Statistics**

Mean length of stay ranged approximately from 2.8 to 6.1 days across groups

Emergency admissions accounted for a high proportion (>95%) of admissions across most ethnic categories

Mean age varied substantially between groups, which may partially explain observed differences in length of stay

**Limitations**

Analysis is based on aggregated data, preventing individual-level inference.

No adjustment for comorbidities, diagnosis, or socioeconomic factors

Observed associations are descriptive, not causal

**Conclusion**

This analysis demonstrates meaningful variation in hospital length of stay across ethnic categories within NHS Admitted Patient Care data. Groups with higher proportions of emergency 
admissions tended to experience longer average hospital stays, highlighting the importance of admission pathways when interpreting population-level hospital utilisation patterns.

The findings emphasise the value of routinely collected administrative data for health services research while underscoring the need for cautious interpretation when individual-level clinical detail is unavailable.

 **Tools Used**

Python

pandas

matplotlib

seaborn

Jupyter Notebook

 **Repository Contents**

01_hes_analysis.ipynb — Full analysis notebook

mean_los_by_ethnicity_top15.png — Figure 1: Mean length of stay

emergency_prop_vs_mean_los.png — Figure 2: Emergency admissions vs LOS

ethnicity_los_summary.csv — Summary statistics table

- seaborn
