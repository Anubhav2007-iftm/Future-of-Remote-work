📊 Future of Remote Work: Productivity Analysis during the COVID-19 Pandemic
📝 Overview
The COVID-19 pandemic has fundamentally shifted the way organizations operate, making remote work a preferred and necessary arrangement. While remote work offers benefits such as cost savings, increased diversity, and inclusion, it also raises concerns over mental burnout and reinforcement of traditional gender norms — particularly for younger employees.

This project explores two core questions:

What factors influence employees' perceived productivity under remote work conditions?

How do employers benefit from implementing remote work systems?

📂 Dataset Summary
The data was sourced from two surveys conducted by the New South Wales Government during:

August–September 2020

2021

After combining similar questions from both datasets and performing thorough preprocessing, the final dataset included:

2,804 rows and 29 columns

Target Variable: Perceived Productivity (Low, Same, High)

Input Variables:

Numeric: % remote work in 2020, preferred % remote work

Categorical: Gender, Occupation Description

🔧 Data Preprocessing Steps
Removed rows with missing values and respondents aged 67 or older

Encoded categorical variables numerically

Scaled ordinal variables appropriately

Handled outliers using the 3σ rule, replacing them with median values

Split data into 70% training and 30% validation

🧠 Methodology
Model Used: Random Forest Classifier

Performance Metrics:

Validation Accuracy: 60.69%

Training Accuracy: 77.42%

Ordinal Accuracy: 83.39%

Mean Absolute Error: 0.52

Despite attempts to mitigate class imbalance via sampling and alternative models, the random forest remained the best-performing model.

🔍 Feature Importance & Analysis
The top factors influencing remote work productivity (in descending order):

Preference for remote work

Age

Daily remote work hours

In-person commuting time

Ease of collaboration while remote

Prior remote work experience in 2020

Time spent on family/domestic responsibilities

Further insights revealed that occupation type significantly influences productivity perception. For example, managerial roles, corporate/public professionals, and sales workers reported increased productivity with remote work.

📈 Partial Dependence Plots
Used to isolate and visualize the effect of individual features on perceived productivity.

💡 Key Recommendations
To maximize productivity in remote settings, organizations should:

Encourage flexible work agreements

Provide tools for seamless online collaboration

Promote work-life balance initiatives

Identify and mitigate remote work barriers

Offer age-specific support programs

