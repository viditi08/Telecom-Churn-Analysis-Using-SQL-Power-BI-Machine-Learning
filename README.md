"Telecom-Churn-Analysis-Using-SQL-Power-BI-Machine-Learning" 

Introduction

In today’s competitive business environment, retaining customers is crucial for long-term success. Churn analysis is a key technique used to understand and reduce customer attrition. This project focuses on examining customer data to identify patterns and reasons behind customer departures. Using advanced data analytics and machine learning, businesses can predict which customers are at risk of leaving and take proactive steps to improve customer satisfaction and loyalty.

Project Goals

The objective of this project is to build an end-to-end churn analysis system that includes:

ETL Process: Extract, transform, and load (ETL) customer data into a SQL Server database.

Power BI Dashboard: Visualize customer data, analyze churn trends, and predict future churners.

Churn Prediction Model: Use machine learning (Random Forest) to predict customer churn based on historical data.

Technologies Used

Database: Microsoft SQL Server, SQL Server Management Studio (SSMS)

Visualization: Power BI

Programming: Python (Jupyter Notebook, Pandas, Scikit-learn)

Machine Learning Model: Random Forest Classifier

Project Structure

ETL Process in SQL Server

Install SSMS: Download Here

Create a database: db_Churn

Import CSV data using SQL Server Import Wizard

Set customerId as the primary key and ensure data integrity

Power BI Transformation & Visualization

Load transformed data into Power BI

Create calculated columns and measures:

Total Customers = COUNT(prod_Churn[Customer_ID])

Total Churn = SUM(prod_Churn[Churn Status])

Churn Rate = [Total Churn] / [Total Customers]

Develop dashboards for:

Demographics (Gender, Age Group, Marital Status)

Account Info (Payment Method, Contract, Tenure)

Geographic Analysis (State-wise churn distribution)

Service Usage (Internet type, subscription status)

Churn Prediction Analysis

Machine Learning Model for Churn Prediction

Install Anaconda: Installation Guide

Load data into Jupyter Notebook

Install necessary libraries:

pip install pandas numpy scikit-learn matplotlib seaborn

Train a Random Forest model:

from sklearn.ensemble import RandomForestClassifier
model = RandomForestClassifier(n_estimators=100, random_state=42)
model.fit(X_train, y_train)

Evaluate the model and integrate predictions into Power BI

How to Run the Project

Set Up Database

Install SQL Server & SSMS

Create the database db_Churn

Import CSV data into the database

Power BI Dashboard

Connect Power BI to SQL Server

Import transformed data and create measures

Design dashboard components

Churn Prediction Model

Install Anaconda and Jupyter Notebook

Load churn dataset and preprocess data

Train and evaluate the Random Forest model

Export predictions and visualize in Power BI

Results & Insights

Customer segmentation by demographics, account details, and location

Identification of high-risk churn groups

Predictive insights to inform marketing and retention strategies

Comprehensive dashboard with churn rate, trends, and contributing factors
