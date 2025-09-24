Hepatitis C Virus (HCV) Liver Function Analysis 🩺
This repository contains the analysis of liver function biomarkers in patients with the Hepatitis C Virus (HCV). The study focuses on Alanine Aminotransferase (ALT) levels to assess liver health variability across different demographic and clinical groups. This project was conducted as part of the course 

21AIC401T Inferential Statistics and Predictive Analytics. 

📝 Abstract
This study uses a publicly available dataset to perform an inferential analysis on liver function in HCV patients. We conducted several statistical hypothesis tests—one-sample, two-sample, and one-way ANOVA—to evaluate differences in ALT levels. The findings provide insights into liver health patterns in this patient cohort, which can help guide personalized clinical monitoring. 



📊 Dataset & Methodology

Dataset: A publicly available HCV dataset (hevdat0.csv) with a sample size of 615 patients. 


Variables: The primary variable of interest is ALT. Other variables considered include 

AST, Bilirubin, Albumin, Sex, Age, and Clinical Category. 


Clinical Categories: Patients were classified into five distinct groups: Blood Donor, Suspect Blood Donor, Hepatitis, Fibrosis, and Cirrhosis. 

Statistical Tests:


One-Sample t-test: To compare the mean ALT of the cohort against a reference value of 30 IU/L. 


Two-Sample t-test: To compare the mean ALT between male and female patients. 


One-way ANOVA: To assess differences in mean ALT across the five clinical categories. 


Post-hoc Tukey HSD: To identify specific pairs of categories with significant differences following the ANOVA test. 

📈 Key Findings

One-Sample Test: The mean ALT for the cohort (28.45 IU/L) was not significantly different from the reference value of 30 IU/L (p=0.1323). This suggests that, on average, ALT levels in this group are within normal clinical limits. 




Two-Sample Test: A significant difference in ALT levels was found between sexes (p=0.0001). The mean ALT for 


males (31.73 IU/L) was significantly higher than for females (23.27 IU/L). 



One-way ANOVA: There was a significant variation in ALT levels across the different clinical categories (F=27.63,p<0.0001). This confirms that ALT is a valuable biomarker for monitoring liver health as the disease progresses. 



Post-hoc Test: The Tukey HSD test revealed significant differences between several group pairs, notably showing that patients with advanced liver damage (Fibrosis and Cirrhosis) had notably higher ALT levels compared to healthy individuals (Blood Donors). 


⚠️ Limitations
Missing numeric values were imputed with the column mean, which may introduce slight bias. 

The analysis focused primarily on ALT, while other liver biomarkers were not explored in depth. 

Some clinical categories had smaller sample sizes, which could affect the statistical power and generalizability of the findings for those specific groups. 
