# HR-ANALYTICS-PROJECT

# HR Analytics Project: Employee Survey and Performance Analysis

# Project Overview
This project involves analyzing employee survey data to extract meaningful insights into work culture, job satisfaction, performance, and other factors. The analysis is performed using SQL for querying and summarizing data, and various machine learning models to predict and classify employee performance. Visualization of key findings is done using Power BI.

Table of Contents
Objective
Technologies Used
Data Analysis and Preprocessing
Machine Learning Models
Power BI Visualization
Conclusion

# Objective
The main objective of this project is to query and analyze employee data to gain a deeper understanding of work culture, job satisfaction, performance, and other influential factors. Key goals include:

Analyzing patterns in employee data using SQL queries.
Predicting employee performance using machine learning models.
Visualizing insights and trends through Power BI dashboards.

# Technologies Used

# SQL:
For querying, aggregation, and summarizing employee data.

# Machine Learning: 
Multiple models (Logistic Regression, Decision Tree, Random Forest, Naive Bayes, KNN) were used to predict and classify employee performance.

# Python Libraries:
Pandas: For data manipulation.
Numpy: For numerical operations.
Seaborn & Matplotlib: For data visualization during exploratory data analysis (EDA).
Scikit-learn: For building and evaluating machine learning models.

# Power BI: 
To create dashboards that summarize key insights from the dataset.

# Data Analysis and Preprocessing

# SQL Queries:

# Total Record Count: 
Queried the total number of employees.
# Gender Distribution:
Aggregated gender-wise counts of employees.
# Salary Distribution: 
Identified the second-highest salary in each department.
# Promotion and Tenure: 
Ranked employees based on tenure and promotion data.

# Preprocessing Steps:

# Handling Missing Values: 
Replaced missing data using mean (for numerical variables) and median (for categorical variables).

# Outlier Detection: 
Outliers were identified using the Interquartile Range (IQR) method.

# One-Hot Encoding: 
Converted categorical variables to binary format for machine learning models.

# Exploratory Data Analysis (EDA):
Checked for missing values and outliers.
Correlation analysis to identify relationships between variables.
Used box plots to visualize the spread of data and detect outliers.

# Machine Learning Models
The following machine learning models were applied to classify and predict employee performance:

# Logistic Regression:

Training Accuracy: 79%
Testing Accuracy: 80%
Best suited for linear relationships in the dataset.

# Decision Tree:

Training Accuracy: 99%
Testing Accuracy: 66%
Overfitting was a major issue, resulting in poor testing performance.

# Random Forest:

Training Accuracy: 99%
Testing Accuracy: 77%
A more robust model that can handle overfitting better than a decision tree.

# K-Nearest Neighbor (KNN):

Training Accuracy: 84%
Testing Accuracy: 74%
Simple but slightly underperformed compared to Logistic Regression and Naive Bayes.

# Naive Bayes:

Training Accuracy: 79%
Testing Accuracy: 80%
A fast and efficient model for handling categorical data with assumptions of independence.

# Power BI Visualization

A Power BI dashboard was created to visualize key metrics from the analysis:

# Job Satisfaction:
Count and satisfaction levels were visualized across job roles.
# Work-Life Balance: 
Explored its relationship with years at the company and performance.
# Monthly Income 
Trends: Analyzed income distribution based on job roles and performance.

# Key findings:

There is a positive correlation between job satisfaction and performance ratings.
Employees with a balanced work-life tend to stay longer at the company.
The highest total monthly income was associated with employees who received low recognition, pointing to discrepancies between performance and recognition.

# Conclusion
The project concluded that Logistic Regression and Naive Bayes were the most effective models for predicting employee performance, with accuracy rates of 80%. The Random Forest model showed promise but needs further hyperparameter tuning. Models like Decision Tree and KNN underperformed, suggesting overfitting and insufficient tuning.

Logistic Regression and Naive Bayes are recommended due to their simplicity and efficiency in handling this data.
Power BI provided crucial insights that can help human resources make informed decisions about employee satisfaction and performance trends.


This README serves as an overview of the key components of the HR Analytics Project and can guide anyone interested in understanding the project workflow, methodologies, and conclusions.








