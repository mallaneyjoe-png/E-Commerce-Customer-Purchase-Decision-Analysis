# E-Commerce-Customer-Purchase-Decision-Analysis
Predictive analysis project using customer data from an e-commerce retail company to identify which users are most likely to purchase. The project uses Python to perform Logistical Regression, and Random Forest classification to analyze customer behavior, improve marketing targeting, and uncover key purchase drivers.
# Project Overview
This project analyzes customer data from an e-commerce company to predict whether a customer is likely to make a purchase. Based on the dataset, the company appears to operate in the fashion and retail merchandising space, with customer information related to demographics, income, employment type, product category, time spent, and purchase behavior.
The main objective of this project is to build a machine learning model that can classify customers into two groups:
0 = Customer did not purchase
1 = Customer purchased.
By identifying the factors most associated with purchasing behavior, this analysis can help an e-commerce company improve customer targeting, marketing efficiency, and merchandising strategy.
# Business Problem
E-commerce companies often face challenges converting visitors into paying customers. Without a clear understanding of which customers are most likely to purchase, marketing campaigns may be too broad, inefficient, and expensive.
This project addresses the following question:
# Can we use customer demographic and behavioral data to predict whether a customer will make a purchase?
The insights could help the company:
Identify high-probability buyers
Make marketing campaigns more targetted
Reduce wasted advertising spend
Better understand customer behavior
Support product and merchandising decisions
# Dataset Description
The dataset contains customer-level information for an e-commerce company. The variables include demographic, behavioral, and product-related features.
Key fields include:
Gender
Age
EstimatedSalary
Education_Level
Region
Employment_type
Product_Category
Time_Spent
Num_of_children
Purch_Attention
Purchased
The target variable is Purchased, which indicates whether the customer completed a purchase.
# Data Cleaning and Preprocessing
Before modeling, the dataset was cleaned and prepared for analysis.
The preprocessing steps included:
Removed extra spaces from column names
Checked for missing values
Filled missing numeric values using the median
Filled missing categorical values using the mode
Removed User ID because it is a non-predictive identifier
Separated the data into features and target variable
Encoded categorical variables using one-hot encoding
Split the data into training and testing sets
Median was used for numeric values because it is less affected by extreme values than the mean. Mode was used for categorical values because it replaces missing categories with the most common category in that column.
# Methodology
Loaded and reviewed the e-commerce dataset
Cleaned column names and checked the data structure
Handled missing values using median or mode imputation
Removed non-predictive identifier columns, such as User ID
Separated the dataset into features and target variable
Encoded categorical variables using one-hot encoding
Split the data into training and testing sets
Built a Logistic Regression classification model
Built a Random Forest classification model
Compared both models using accuracy, ROC-AUC, correclation matrix, and classification report
Analyzed feature importance from the Random Forest model to identify key purchase drivers
# Models Used
# Logistic Regression
Logistic Regression was used as a baseline model because it is simple, interpretable, and effective for binary classification problems. Since the target variable is whether a customer purchased or did not purchase, Logistic Regression provides a clear starting point for understanding how customer characteristics relate to purchase probability.
# Random Forest Classifier
Random Forest was used as the primary machine learning model because it can capture more complex relationships in the data. Unlike Logistic Regression, which assumes a more linear relationship between the features and the target, Random Forest uses multiple decision trees to identify patterns that may not be obvious through a simpler model.
# Model Comparison
After training both models, their performance was compared using several classification metrics:
Accuracy: Measures the percentage of correct predictions
Confusion Matrix: Shows correct and incorrect predictions for each class
Classification Report: Provides precision, recall, and F1-score
Using both models allowed the project to compare a simpler, more interpretable model against a more flexible and powerful machine learning model.
This comparison helps answer not only whether customer purchases can be predicted, but also which model provides better performance for this type of business problem.
# Key Objective
Which customers are most likely to purchase, and which model best predicts purchase behavior?
# Business Value
A company could use this type of prediction model to:
Prioritize marketing toward customers with higher purchase probability
Create more personalized campaigns
Improve customer segmentation
Identify which customer characteristics are most connected to conversion
Support more data-driven merchandising decisions
Compare model approaches before choosing one for business use
# Limitations
This project is based on a relatively small dataset, so the results should be interpreted carefully.
Other limitations include:
Some missing values had to be filled using median and mode imputation
Median and mode imputation are practical, but they do not perfectly replace real customer data
The dataset does not include product price, website traffic source, purchase history, discounts, or web cart activity
# Conclusion
This project uses customer data from an e-commerce company to predict whether a customer will make a purchase.
We cleaned the data, filled missing numbers with the median, and filled missing categories with the mode. This helped us keep the full dataset instead of deleting rows with missing information.
We then built two models: Logistic Regression and Random Forest. After comparing them, we used the results to see which model predicted purchases better and what customer factors seemed most connected to buying.
Overall, this project helps show how data can be used to better understand customers and improve marketing decisions.
