# telco_classification_project
---
This repo includes my work and deliverables for our first machine learning project.

## About the Project
---
### Project Goal
The goal of this project is to identify factors that lead to customer churn at Telco and then make recommendations to reduce churn and increase customer retention.

### Project Description
Every month, we are losing customers. When a customer leaves, not only do we lose their monthly payments, we also have to account for the cost of replacing that customer. Keeping our customers needs to be a priority, and so, with this project, I will discover what factors make our customers more or less likely to leave. With that information, I will develop a model for predicting whether or not customers will churn. Finally, I will deliver recommendations and predictions for the future.

### Initial Questions
1. Are customers with higher monthly charges more likely to churn?
2. Is there a relationship between gender and rate of churn?
3. Is there a difference in rate of churn between customers with dependents and customers without dependents?
4. Does whether or not a customer has paperless billing set up affect a customer's likelihood of churn?

### Data Dictionary
| Variable | Meaning |
| -------- | ------- |
| telco    | The full, unsplit telco dataframe |
| train    | A sample (56%) of telco used for exploring data and fitting/training models |
| validate | A sample (24%) of telco used to evaluate multiple models |
| test     | A sample (20%) of telco used to evaluate the best model |
| has_churned | Our target variable: whether or not a customer has churned |
| customer_id | The ID used to distinguish each customer |
| has_paperless_billing | Whether or not a customer is enrolled in paperless billing |
| senior_citizen | Whether or not a customer is a senior citizen |
| tenure   | Number of months a customer has been with Telco |
| monthly_charges | Amount paid by customer each month |
| total_charges | Total amount paid by customer to date |
| is_male | Whether or not a customer is male |
| has_partner | Whether or not a customer has a partner |
| has_dependents | Whether or not a customer has dependents |
| has_phone_service | Whether or not a customer has phone service |
| multiple_lines | Whether a customer has multiple lines (Dummy variables: multiple_lines_Yes, multiple_lines_No phone service)  |
| online_security | Whether a customer is enrolled in online security (Dummy variables: online_security_Yes, online_security_No internet service) |
| online_backup | Whether a customer is enrolled in online backup (Dummy variables: online_backup_Yes, online_backup_No internet service) |
| device_protection | Whether a customer is enrolled in device protection (Dummy variables: device_protection_Yes, device_protection_No internet service |
| tech_support | Whether a customer is enrolled in tech support (Dummy variables: tech_support_Yes, tech_support_No internet service |
| streaming_tv | Whether a customer has streaming tv (Dummy variables: streaming_tv_Yes, streaming_tv_No internet service) |
| streaming_movies | Whether a customer has streaming movies (Dummy variables: streaming_movies_Yes, streaming_movies_No internet service) |
| contract_type | What type of contract the customer has. Options are one-year, two-year, and month-to-month. (Dummy variables: contract_type_One year, contract_type_Two year) |
| internet_service_type | What type of internet service the customer has. Options are Fiber optic, DSL, or None (no internet service). (Dummy variables: internet_service_type_Fiber optic, internet_service_type_None) |
| payment_type | How the customer pays their bill. Options are Credit card (automatic), Mailed check, Electronic check, and Bank transfer (automatic). (Dummy variables: payment_type_Credit card (automatic), payment_type_Electronic check, payment_type_Mailed check) |

### Steps to Reproduce
- In a local repository, create an env.py file to store the hostname, username, and password that will be used to access the mySQL database containing the telco data.
- Clone this repository, making sure the .gitignore is successfully hiding the env.py file.
- Run all cells in Report.ipynb.
- If desired, run all cells in the other Jupyter notebooks (wrangling.ipynb, exploration.ipynb) in this repository to see my full, in-depth step-by-step process for this project.

### The Plan

#### Wrangle

1. Define a function to acquire the telco data from the mySQL database.
2. Define a function to clean the acquired telco data.
3. Define a function to split the cleaned telco data.
4. Define a function to combine the previous 3 steps into a single function.
5. Ensure all functions work properly and add them to telco_functions.py file.

#### Explore
1. Ask a clear question.
2. Develop null and alternative hypotheses for that question.
3. Use visualizations and statistical tests to find answers.
4. Clearly state the answer to the question and summarize findings.
5. Repeat for a total of at least 4 questions.
6. Summarize key findings, takeaways, and actions.

#### Model
1. Select a metric to use for evaluating models and explain why that metric was chosen.
2. Create and evaluate a baseline model.
    - Find most common outcome (churned or not churned)
    - Set all predictions to that outcome
    - Evaluate based on selected evaluation metric
3. Develop three models.
4. Evaluate all three models on the train sample, note observations.
5. Evaluate the top two models on the validate sample, note observations.
6. Evaluate the top performing model on the test sample, note observations.
7. Create a .csv file of predictions made on the test sample by the top performing model.

#### Deliver
1. Ensure final report notebook is thoroughly code commented.
2. Ensure notebook contains enough Markdown cells to guide the reader through the report.
3. Write a conclusion summary.
4. Develop actionable recommendations for the business.
5. Suggest next steps for research and/or model improvement.
6. Run final report notebook from beginning to be sure that there are no errors.
7. Submit link to repository containing project files.
8. Deliver live presentation.
