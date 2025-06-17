The Future of Work: Analyzing Employee Productivity in a Remote World
📊 An analysis of the factors influencing employee productivity and employer benefits in a remote work environment, based on survey data from the COVID-19 pandemic era.
📌 Overview
The COVID-19 pandemic catalyzed a global shift to remote work, presenting both opportunities and challenges for employers and employees. While remote work offers benefits like increased diversity, inclusion, and cost savings, it also raises concerns about reinforcing gender norms and potential employee burnout.
This project investigates the dynamics of remote work by analyzing data from two surveys conducted by the New South Wales government in 2020 and 2021. Using a Random Forest model, we identify the key drivers of perceived productivity and provide data-driven recommendations for organizations navigating the future of work.
🎯 Research Questions
This study aims to answer two primary questions:
What factors most significantly affect an employee's perceived productivity in a remote work setting?
How do employers benefit from implementing remote work systems?
💾 The Dataset
The data for this project was sourced from two surveys conducted by the authorities of New South Wales to understand remote workers' experiences.
Source: Two surveys from 2020 and 2021.
Target Variable: Perceived Productivity (Categorical: Low, Same, High).
Features: A mix of numeric (e.g., preferred remote work %) and categorical (e.g., occupation) variables.
Final Size: After preprocessing, the dataset contains 2,804 samples and 29 features.
⚙️ Methodology
The analysis followed a structured data science workflow:
1. Data Preprocessing
Data Combination: Questions from both surveys were merged.
Data Cleaning:
Rows with missing values were removed.
Unnecessary columns were dropped.
Respondents aged 67 or older were excluded.
Feature Engineering:
Categorical variables were numerically encoded.
Scaled responses were transformed into ordinal scales.
Outlier Handling: Outliers identified using the 3-standard-deviation rule were replaced with the column median.
Data Splitting: The data was split into a 70% training set and a 30% validation set.
2. Modeling and Analysis
Classification Model: A Random Forest Classifier was trained to predict the three classes of Perceived Productivity.
Feature Importance: The model's feature importance scores were extracted to identify the most influential factors.
Partial Dependence Plots (PDP): PDPs were used to isolate and visualize the relationship between the top features and productivity.
📈 Model Performance
The Random Forest model achieved the following results on the validation set:
Metric	Score
Accuracy	60.69%
Ordinal Accuracy	83.39%
Mean Absolute Error	0.52
Training Accuracy	77.42%
Note: While a class imbalance was identified, alternative models and sampling techniques did not yield superior results.
💡 Key Findings: Top Factors Influencing Productivity
The feature importance analysis revealed the top factors that influence an employee's perceived productivity when working remotely, in descending order of importance:
Strong Preference for Remote Work: Employees who want to work remotely are more productive.
Age: The age of the employee plays a significant role.
Daily Remote Work Hours: The number of hours spent working remotely per day.
In-Person Commute Time: Longer commute times saved correlated with higher productivity.
Ease of Collaboration: Employees who found online collaboration easy were more productive.
Prior Remote Work Experience: Experience with remote work during 2020 was a key factor.
Time Gained for Personal Life: Hours saved that could be used for family or domestic duties.
Occupation Type: Roles like "Managerial" or "Technician" showed different attitudes and productivity outcomes.
Deeper analysis showed that productivity particularly rose for Managerial Positions, Corporate and Public Sector Professionals, and Sales Workers.
🚀 Recommendations for Employers
To enhance productivity and leverage the benefits of remote work, employers should:
Promote Flexible Work Agreements: Allow employees to choose work arrangements that suit them best.
Invest in Collaboration Tools: Provide technology that makes virtual teamwork seamless and effective.
Encourage Work-Life Balance: Actively support employees in disconnecting and managing their time.
Address Remote Work Barriers: Identify and help employees overcome individual challenges with remote work.
Provide Tailored Support: Recognize that different demographics (especially age groups) may require different types of support to thrive.
