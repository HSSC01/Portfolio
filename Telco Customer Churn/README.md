# Telco Customer Churn Analysis
Chosen project for the IBM Exploratory Data Analysis in Machine Learning course Honors Module and IBM Supervised Machine Learning: Classification course Final Project.
## Description
Exploratory Data Analysis (EDA)
This section of the project focuses on analysing customer churn in a telecommunications company using EDA, feature engineering, and statistical tests. The goal was to uncover patterns and relationships in customer behaviour, such as the influence of customer demographics, service usage, and contract types on churn. Insights gained from this analysis helped inform the subsequent machine learning modeling process.

Final Project - Supervised Machine Learning: Classification
For the final project, the objective was to predict customer churn using machine learning classification models. Three different classifiers were trained: Logistic Regression, Random Forest Classifier, and Support Vector Classifier (SVC). After evaluating the performance of all models, the Random Forest Classifier was selected as the final model, achieving an accuracy of 79%. This model demonstrated strong precision and recall, particularly in predicting customers who are likely to churn. The final choice was based on the model's accuracy, interpretability, and its ability to highlight important features related to churn.

## Technologies Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Dataset Description
The dataset contains the following features:
- CustomerID
- Gender
- SeniorCitizen
- Partner
- Tenure
- MonthlyCharges
- TotalCharges
- Churn (Target Variable)

## Steps Taken
- Data Cleaning: Handled missing values and encoded categorical variables.
- Exploratory Data Analysis (EDA): Analysed correlations and visualised relationships.
- Feature Engineering: Created new features such as 'Tenure Group' and 'Monthly Charges per Tenure'.
- Hypothesis Testing: Conducted a Chi-Square test on the relationship between contract type and churn.

## Conclusion
- High churn rate is observed in customers with month-to-month contracts.
- Senior Citizens have a higher churn rate than non-Senior Citizens.
- Customers with fewer services (e.g., no tech support or device protection) tend to churn more.

## Files in this Repository
- **Code**: Contains Python scripts for data analysis and visualisation (`code/`).
- **PowerPoint Presentation**: Summarizes the project findings (`presentation/`).
- **Dataset**: The raw Telco customer churn data (`data/`).
