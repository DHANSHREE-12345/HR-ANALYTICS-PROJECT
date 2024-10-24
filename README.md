# HR-ANALYTICS-PROJECT

# Introduction and Context:
The project is focused on analyzing employee survey data to gain insights into their work environment, job satisfaction, performance, and more. The dataset includes a range of employee details such as:

Employee ID, Age, Location, Job Role
Work-Life Balance, Promotions, Work Experience

This data forms the basis for understanding the work culture, and influences that impact employees' job satisfaction and performance.
The project involved analyzing an employee survey dataset containing various features, such as employee demographics (age, gender, job role, work experience), job satisfaction levels, promotions, work-life balance, and performance ratings. The goal was to extract valuable insights using both data querying techniques in SQL and advanced machine learning algorithms. Power BI was used to create a dashboard for summarizing the data visually, making insights easier to understand and act upon.

# Project Objective:
The key goal is to extract meaningful insights from this survey data by:

# Data Analysis and SQL Queries:

# To analyze the dataset, SQL was used extensively:

# Counting Records: 
The total number of records was counted using SELECT COUNT(*) FROM train.
# Gender Distribution:
The distribution of employees by gender was analyzed using SELECT gender, COUNT(Employee_ID) FROM train GROUP BY gender.
# Promotion and Tenure Analysis:
Employees were ranked based on tenure and promotions to identify top performers.
# Salary Analysis: 
SQL queries were used to find employees with the second-highest salary in each department. These queries helped identify key trends such as gender distribution, promotion rates, and salary variations across departments.

# Data Preprocessing:

# Handling Missing Data: 
Missing values were replaced using the mean (for numerical variables) and median (for categorical variables).
# Outliers Detection:
Outliers were identified using Interquartile Range (IQR). Outliers in the dataset were managed by calculating the upper and lower limits of data variability.
# One-Hot Encoding for Categorical Variables: 
Categorical variables (such as job role, location, etc.) were converted into a binary format for better use in machine learning algorithms.
# Machine Learning Models Applied:
Multiple supervised learning models were used to classify and predict employee performance, job satisfaction, and other outcomes.

# Logistic Regression:

Training Accuracy: 79%
Testing Accuracy: 80%
Logistic regression was used for classification, particularly because the problem involved predicting categorical variables (e.g., job satisfaction).

# Decision Tree Classifier:

Training Accuracy: 99%
Testing Accuracy: 66%
The Decision Tree classifier was used for classification tasks but showed signs of overfitting, which caused a significant drop in testing accuracy.

# Random Forest Classifier:

Training Accuracy: 99%
Testing Accuracy: 77%
This model combines multiple decision trees, improving performance but requiring further optimization for better testing results.

# K-Nearest Neighbor (KNN):

Training Accuracy: 84%
Testing Accuracy: 74%
KNN was used due to its simplicity but did not outperform other models, suggesting that further tuning or preprocessing could improve results.

# Naive Bayes:

Gaussian NB, Multinomial NB, Bernoulli NB were applied:
Training Accuracy: 79%
Testing Accuracy: 80%
Naive Bayes performed well in terms of accuracy and simplicity, making it a viable model for prediction in this context.

# Correlation Analysis:

# Correlation Matrix: 
The analysis identified correlations between different variables (e.g., performance status, job satisfaction, work-life balance, income).
# Heatmap Visualization:
A heatmap was generated to visualize how various factors correlated with employee performance, helping the team identify strong relationships between variables.

# Comparison of Machine Learning Models:

Based on accuracy comparisons, Logistic Regression and Naive Bayes performed best with 80% accuracy, showing their potential in solving the problem at hand, especially where the relationships were linear or feature independence was important.
Random Forest showed good performance but did not significantly outperform simpler models.
Decision Tree and KNN underperformed, with the Decision Tree model being particularly affected by overfitting.

# Power BI Dashboard Insights:
The team developed a Power BI dashboard to visually summarize the results of the analysis:

# Job Satisfaction:
Employee satisfaction was analyzed, revealing that 29,716 employees had the highest count of job satisfaction.
Satisfaction was positively correlated with performance ratings, showing that higher satisfaction levels led to better performance.

# Work-Life Balance and Years at Company:
Employees with a “Good” work-life balance had the highest sum of years at the company, indicating that those with a balanced work-life tend to stay longer.

# Monthly Income and Job Roles:
Income distribution was categorized by job roles, and it was found that employees with lower recognition still had a high percentage of total income, while those with "low" job satisfaction had the highest total monthly income, indicating discrepancies between income and recognition.

# Detailed Conclusion:

# Best Performing Models:

Logistic Regression and Naive Bayes emerged as the best-performing models, particularly useful for handling this type of employee data where relationships are linear.

# Potential for Random Forest:

While Random Forest did not perform as well as expected, further hyperparameter tuning could enhance its performance. However, its complexity suggests that it may not offer significant gains over simpler models like Logistic Regression and Naive Bayes.

# Challenges with Decision Tree and KNN:

The Decision Tree model's significant drop in testing accuracy indicates overfitting, likely due to the model being too complex for the dataset.
KNN also did not perform as well, indicating that while it can be useful for classification problems, it may not be suited for this particular dataset without further tuning.

# Recommendations:

# Focus on Simpler Models: 
Given the results, simpler models like Logistic Regression and Naive Bayes are preferable due to their high accuracy and faster processing times.

# Further Optimization:
Models like Random Forest could be further explored with hyperparameter tuning to assess if significant gains can be made.

# Addressing Overfitting: 
Preprocessing techniques to address overfitting in models like Decision Tree could be explored to improve generalization.

# Visualization: 
Power BI dashboards were crucial in conveying key insights, and continued use of such tools can help in real-time monitoring and decision-making regarding employee performance.
This project provided critical insights into employee behavior, satisfaction, and performance, which can be used to guide human resource decisions and organizational improvements.

# Conclusion:
The project successfully used machine learning and SQL to derive meaningful insights from the employee survey dataset. Logistic Regression and Naive Bayes proved to be the best models for predicting outcomes related to job satisfaction and performance, with Random Forest offering potential if further tuned. The insights generated through SQL queries and Power BI visualization helped highlight key factors like gender distribution, salary trends, and work-life balance impacts, which can inform decision-making in human resource management.

This comprehensive approach combined data-driven analysis with visual storytelling to provide a clear understanding of employee dynamics in the workplace.
