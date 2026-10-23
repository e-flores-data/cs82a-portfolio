Maternal Health Risk Analysis
Question: How does average age, blood pressure, and blood sugar compare across the different risk groups?

Data:
This project uses the Maternal Health Risk dataset from the UCI Machine Learning Repository. The data was collected from hospitals, community clinics, and maternal healthcare facilities in rural Bangladesh.

The CSV used for this analysis contains 1,014 rows and seven columns. The variables used in the analysis are:

Age: Age in years

SystolicBP: Systolic blood pressure in mmHg

DiastolicBP: Diastolic blood pressure in mmHg

BS: Blood sugar in mmol/L

RiskLevel: Low, mid, or high maternal health risk

Source: UCI Maternal Health Risk Dataset

License: Creative Commons Attribution 4.0 International (CC BY 4.0)

Cleaning

I checked the dataset’s shape, missing values, and exact duplicate rows. The dataset had no missing values. There were 562 rows with identical values. I could not determine whether the rows represented accidental duplicates or different patients with the same measurements, I kept all observations.

Analysis

I grouped the data by risk level and calculated the average age, systolic blood pressure, diastolic blood pressure, and blood sugar for each group. The dataset contained 406 low-risk records, 336 mid-risk records, and 272 high-risk records.

Findings

Average Age: The high-risk group had the highest average age at 36.22 years. The mid-risk group averaged 28.36 years, while the low-risk group had the lowest average age at 26.87 years.

Average Blood Pressure: Average systolic and diastolic blood pressure increased across the risk groups. The high-risk group averaged 124.19 mmHg systolic and 85.07 mmHg diastolic. The low-risk group averaged 105.87 mmHg systolic and 72.53 mmHg diastolic.

Average Blood Sugar: The high-risk group had the highest average blood sugar level at 12.12 mmol/L. The mid-risk group averaged 7.80 mmol/L, while the low-risk group averaged 7.22 mmol/L.



Conclusion: The high-risk group had the highest average age, systolic blood pressure, diastolic blood pressure, and blood sugar. The results show that higher averages for these measurements are associated with higher recorded maternal health risk levels in this dataset. The analysis describes relationships within the data but does not prove that any measurement caused the risk classification.

Limitations: 
-The data was collected from healthcare facilities in rural Bangladesh, so the results may not represent pregnant patients in other locations. 
-The risk groups contained different numbers of records with different averages. The high risk group had the lowest at 272 so being a smaller value means it can shift more versus a larger group number is not as influenced.




Project Files

maternal_health_analysis.ipynb: Complete analysis

maternal health risk data set.csv: Source data

average_age_by_risk.png: Age chart

average_blood_pressure_by_risk.png: Blood-pressure chart

average_blood_sugar_by_risk.png: Blood-sugar chart

ai_prompt_log.md: Record of AI assistance

References

Ahmed, M. (2020). Maternal Health Risk [Dataset]. UCI Machine Learning Repository.
https://doi.org/10.24432/C5DP5D

AI Disclosure

I used ChatGPT to help with Python syntax, chart formatting, organizing the notebook and README, and clarifying my own explanations. The complete AI prompt log is included in folder.
