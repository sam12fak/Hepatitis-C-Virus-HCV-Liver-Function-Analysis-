# 🩺 Hepatitis C Virus (HCV) Liver Function Analysis

This repository contains the analysis of liver function biomarkers in patients with the Hepatitis C Virus (HCV).  
The study focuses on **Alanine Aminotransferase (ALT)** levels to assess liver health variability across different demographic and clinical groups.  

This project was conducted as part of the course:  
**21AIC401T – Inferential Statistics and Predictive Analytics**



## 📝 Abstract
This study uses a publicly available dataset to perform an **inferential analysis** on liver function in HCV patients.  
We conducted several statistical hypothesis tests—**one-sample, two-sample, and one-way ANOVA**—to evaluate differences in ALT levels.  

The findings provide insights into liver health patterns in this patient cohort, which can help guide personalized clinical monitoring.



## 📊 Dataset & Methodology

- **Dataset**: A publicly available HCV dataset (`hcvdat0.csv`) with a sample size of **615 patients**.  
- **Primary Variable**: `ALT`  
- **Other Variables**: `AST`, `Bilirubin`, `Albumin`, `Sex`, `Age`, and `Clinical Category`  

### Clinical Categories
Patients were classified into five distinct groups:
- Blood Donor  
- Suspect Blood Donor  
- Hepatitis  
- Fibrosis  
- Cirrhosis  

### Statistical Tests
1. **One-Sample t-test** → Compare mean ALT against reference value of 30 IU/L  
2. **Two-Sample t-test** → Compare mean ALT between male and female patients  
3. **One-way ANOVA** → Assess differences in mean ALT across the five clinical categories  
4. **Post-hoc Tukey HSD** → Identify specific category pairs with significant differences  



## 🛠️ Tools & Libraries Used
- **Python**
  - pandas → Data manipulation & cleaning  
  - numpy → Numerical computations  
  - matplotlib → Data visualization  
  - seaborn → Statistical visualization  
  - scipy → Hypothesis testing  
  - statsmodels → ANOVA & post-hoc analysis  



## 📈 Key Findings

- **One-Sample Test**  
  - Mean ALT = **28.45 IU/L**  
  - Not significantly different from reference value 30 IU/L *(p = 0.1323)*  
  - Suggests ALT levels are within normal clinical limits on average  

- **Two-Sample Test**  
  - Significant difference between sexes *(p = 0.0001)*  
  - Males: **31.73 IU/L** vs Females: **23.27 IU/L**  

- **One-way ANOVA**  
  - Significant variation across categories *(F = 27.63, p < 0.0001)*  
  - Confirms ALT as a useful biomarker for monitoring disease progression  

- **Post-hoc Tukey HSD**  
  - Patients with **Fibrosis & Cirrhosis** had significantly higher ALT levels than **Blood Donors**  



## ⚠️ Limitations

- Missing numeric values were imputed with the column mean → may introduce slight bias  
- Focused primarily on **ALT**, other biomarkers (AST, Bilirubin, Albumin) not explored in depth  
- Some categories had smaller sample sizes → may affect statistical power & generalizability  
