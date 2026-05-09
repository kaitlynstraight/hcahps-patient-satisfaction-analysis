# HCAHPS Patient Satisfaction Analysis   
An exploratory data analysis and predictive modeling project examining which hospital characteristics predict patient satisfaction scores across 4,789 U.S. hospitals, using publicly available CMS data.   

**Motivation**   
Inspired by supply chain work at Kaiser Permanente and an interest in post-market surveillance analytics, this project investigates whether public data sources can surface patterns in patient experience, and what operational and structural hospital characteristics influence overall patient satisfaction.    

**Data Sources**
- HCAHPS Hospital Survey (CMS Provider Data Catalog) — *patient satisfaction scores across 4,789 hospitals, April 2024 – March 2025*    
- Hospital General Information (CMS Provider Data Catalog) — *hospital characteristics including ownership type, hospital type, mortality measures, safety measures, and readmission rates*    

**Research Questions**    
- Which patient experience measures most strongly predict overall hospital ratings?    
- Do hospital ownership type and size affect patient satisfaction scores?    
- Do clinical quality measures (mortality, safety, readmissions) correlate with patient satisfaction?    

**Analysis**    
Data cleaning and reshaping from long to wide format across 325,652 survey responses   
Correlation analysis across satisfaction measures   
Exploratory analysis by ownership type and hospital type   
Scatter plot analysis of clinical quality vs satisfaction   
Linear Regression model (R² = 0.904, RMSE = 2.63pp)   
Random Forest model for feature importance validation   

**Key Findings and Recommendations**   
**_Nurse communication and patient recommendation rates_** are the dominant predictors of overall satisfaction — far outweighing clinical quality measures.   
Critical Access hospitals consistently outperform Acute Care hospitals on patient satisfaction despite generally having fewer resources.   
Mortality, safety, and readmission measures have near-zero correlation with satisfaction scores, confirming that _patient experience captures a fundamentally different aspect of care than clinical outcomes._   
VA/DOD hospitals outperform expectations on satisfaction compared to private hospitals.    
Nonprofit vs for-profit ownership has minimal impact on satisfaction scores.    

**Tools**   
Python · Pandas · Scikit-learn · Matplotlib · Seaborn · Jupyter Notebook    

**Visualizations**    
<img width="2383" height="1535" alt="hcahps_distributions" src="https://github.com/user-attachments/assets/243cce5d-9130-45dd-8f18-db9868cb1d41" />    
<img width="1280" height="1182" alt="hcahps_correlation" src="https://github.com/user-attachments/assets/83c0db48-f181-4ed3-b919-039db3643429" />    
<img width="2383" height="888" alt="satisfaction_by_ownership" src="https://github.com/user-attachments/assets/4d2e16e4-77fe-47c0-8816-d8e405d5cac0" />    
<img width="2383" height="888" alt="satisfaction_by_hospital_type" src="https://github.com/user-attachments/assets/a628f8bb-1aa4-4301-a177-e3815c94617a" />    
<img width="2383" height="1476" alt="satisfaction_vs_quality" src="https://github.com/user-attachments/assets/21ac9a03-efa2-4f22-b165-f12f14096f85" />    
<img width="1484" height="1185" alt="regression_coefficients" src="https://github.com/user-attachments/assets/d86865a5-2955-4209-bc47-2a7431b30b5f" />
