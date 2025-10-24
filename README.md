# GRADUATE-EMPLOYABILITY-RATE
Conducted an end-to-end data analysis to identify factors influencing graduate employment outcomes. Cleaned and transformed data in Excel, performed regression analysis to predict employability, and visualized insights in Power BI. Findings revealed that project completed and IQ levels were strong predictors of employability success.


📘 Project Overview

This project explores the key factors that influence graduate employability, using a dataset obtained from Kaggle
. The aim is to uncover relationships between academic performance, technical skills, soft skills, and internship experience, and how these variables impact the likelihood of employment after graduation.

The analysis was performed using Excel and Power BI, combining statistical techniques and data visualization to communicate actionable insights.

🎯 Objectives

Determine the overall employability rate among graduates.

Analyze the impact of internship experience on employability.

Examine how academic performance (CGPA) affects employment outcomes.

Assess the influence of soft skills (e.g., communication, teamwork) on employability.

Use regression analysis to predict employability based on technical skills (IQ, projects completed, etc.).

🧩 Dataset Information

Source: Kaggle – Graduate Employability Dataset

Records: ~10,000 graduates

Key Features:


CGPA

Internship Experience (Yes/No)

Technical Skills (IQ, Projects Completed)

Soft Skills (Communication, Teamwork)

Employment Status (1 = Employed, 0 = Unemployed)

🧹 Data Cleaning & Preparation

Performed in Excel:

Removed duplicates and null values

Standardized text responses (Yes/No → 1/0)

Created derived variables (e.g., CGPA Category)

Verified data consistency across all records

📊 Exploratory Data Analysis (EDA)

Conducted using Excel Pivot Tables and Power BI:

Employability distribution across technical skills and soft skills

Internship vs Employment comparison

CGPA trends among employed vs unemployed graduates

Skill correlation analysis with employment status



📈 Regression Analysis


Tools Used
Excel: For data cleaning, preliminary analysis, and running regression models.
Power BI: For advanced data visualization to uncover insights and present findings effectively.


🔍 What i did

I performed a multiple linear regression to predict Employability (Placement Outcome) based on seven predictor variables:

IQ

CGPA

Academic Performance

Internship Experience

Extra-Curricular Score

Communication Skills

Projects Completed

📊 2. Model Summary
Metric	Meaning	Interpretation
Multiple R = 0.5827	Correlation between actual and predicted employability	There is a moderate positive relationship (≈58%) between your predictors and employability.
R Square = 0.3395	Proportion of variance explained by the model	Your predictors explain ≈34% of the variation in employability outcomes.
Adjusted R² = 0.3390	Adjusted for number of predictors	After adjusting for the number of variables, your model still explains ≈33.9% of employability variation — meaning the model is fairly solid.
Standard Error = 0.3024	Average error of prediction	The typical prediction error is around 0.30, which is acceptable given your dataset size (10,000 observations).

📈 3. ANOVA Table
Source	df	SS	MS	F	Significance F
Regression	7	469.81	67.12	733.74	0.000
Residual	9992	913.97	0.091		
Total	9999	1383.77			

F = 733.74, Significance F = 0.000 →
🔹 This means your overall regression model is statistically significant (p < 0.05).
In simple terms, your independent variables collectively explain employability meaningfully.

📉 4. Coefficients Table Interpretation
Variable	Coefficient	P-Value	Interpretation
Intercept = -1.504	—	—	When all predictors are 0, employability baseline is negative (not interpretable directly, serves as model constant).
IQ = 0.0071	6.6e-258	✅ Significant	Each unit increase in IQ increases employability likelihood by 0.7%, keeping others constant.
CGPA = 0.0821	0.000	✅ Highly significant	A higher CGPA strongly improves employability. Each 1-point increase in CGPA adds 8.2% employability likelihood.
Academic_Performance = -0.00036	0.735	❌ Not significant	No meaningful impact on employability.
Internship = 0.0056	0.367	❌ Not significant	Internship alone doesn’t strongly predict employability, perhaps because many already had internships.
Extra_Curricular_Score = -0.00122	0.201	❌ Not significant	No strong evidence that extracurricular activities directly improve employability.
Communication_Skills = 0.0427	0.000	✅ Highly significant	Very influential — a one-point improvement in communication increases employability by 4.3%.
Projects_Completed = 0.0451	5.76e-140	✅ Highly significant	Completing more projects strongly improves employability by 4.5% per project.


🧠 5. Key Insights

Significant Predictors

✅ CGPA

✅ Communication Skills

✅ Projects Completed

✅ IQ

These have p-values < 0.05, meaning they significantly affect employability.

Non-significant Predictors

❌ Academic Performance

❌ Internship

❌ Extra-Curricular Score

These did not have strong predictive power when combined with other factors.

Most Influential Factors

Communication Skills and Projects Completed have the largest positive coefficients, showing that practical and interpersonal skills drive employability more than academic record alone.


📘 6. Practical Interpretation

Graduates who maintain a high CGPA, complete more real-world projects, and demonstrate strong communication skills are significantly more employable.
IQ also plays a role, but soft skills and applied experience seem to matter just as much as raw intelligence.



💡 Data Insights and Recommendations

Key Insights:

📈 Academic Excellence + Practical Exposure = Employability Boost
Graduates with higher CGPA and more completed projects show significantly higher employability outcomes, confirming the combined importance of knowledge and hands-on experience.

🗣️ Communication Skills are Game-Changers
Strong communication skills consistently predict higher employability, underscoring employers’ growing preference for candidates who can express ideas clearly and collaborate effectively.

🧠 IQ Contributes, But Soft Skills Matter More
While intelligence (IQ) influences employability, the model suggests that soft skills and applied learning experiences have stronger predictive power.

🎓 Internships and Extracurricular Activities Have Limited Predictive Impact
These factors alone do not guarantee employability, possibly due to variations in internship quality or lack of clear alignment with job requirements.

Recommendations:

Integrate Soft Skills into Academic Curricula — Institutions should embed communication and teamwork modules into learning programs.

Encourage Project-Based Learning — Students should be exposed to real-world projects to bridge the gap between theory and practice.

Strengthen Career Readiness Programs — Universities and training centers should focus on employability workshops, CV building, and mock interviews.

Improve Internship Quality — Emphasis should be placed on meaningful, skill-based internships rather than short-term attachments.

Data-Driven Graduate Support — Continuous data tracking on graduate performance can help institutions adjust programs to improve employability outcomes.

📊 Power BI Dashboard

An interactive Power BI dashboard was developed to visualize insights and patterns:

✅ Employability Rate Overview

✅ Internship Impact Analysis

✅ CGPA vs Employability Column Chart

✅ Skill Ratings Comparison





