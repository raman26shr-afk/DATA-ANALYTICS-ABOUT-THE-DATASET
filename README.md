# DATA-ANALYTICS-ABOUT-THE-DATASET

# AIM

To perform data analytics on a given dataset using Python and Pandas, understand the characteristics of the dataset, identify different types of data, examine missing values, and prepare the dataset for further analysis and machine learning.

# THEORY
Data analytics is the process of examining, cleaning, transforming, and interpreting data to discover useful information and patterns. In Artificial Intelligence and Machine Learning, data analytics helps us understand the quality and structure of datasets before building predictive models.

Python is a popular programming language used for data analysis because of its simple syntax and extensive libraries.

Pandas is a Python library used for data manipulation and analysis. It provides two important data structures:

Series: A one-dimensional labeled data structure.

DataFrame: A two-dimensional table containing rows and columns.

# OBJECTIVES

The main objectives of this experiment are:

To understand the structure and characteristics of a dataset.

To learn how to use Python and Pandas for data analysis.

To identify numerical and categorical data.

To detect missing values and duplicate records.

To perform basic data cleaning and preprocessing.

To generate statistical summaries from the dataset.

To prepare data for Machine Learning applications.

To understand the importance of Exploratory Data Analysis (EDA).

# Importance of Data Analytics in AI

Helps understand the structure of a dataset.

Identifies missing and duplicate values.

Detects incorrect or inconsistent data.

Helps identify numerical and categorical features.

Supports data cleaning and preparation.

Improves the quality of data used for machine learning.

# REQUIREMENTS
Hardware Requirements:

Computer or laptop.

Minimum 4 GB RAM.

Keyboard and mouse.

Software Requirements:

Python 3.x.

Jupyter Notebook or Google Colab.

Pandas library.

NumPy library (optional).

# PROCEDURE

Open Jupyter Notebook or Google Colab.

Import the Pandas library.

Create or load a dataset using a CSV file.

Display the first and last few rows of the dataset.

Identify the number of rows and columns.

Examine the data types of each column.

Generate statistical summaries of numerical data.

Identify missing values and duplicate records.

Perform basic data cleaning.

Prepare the dataset for further analysis and machine learning.

# PROGRAM

The following Python program creates a sample student dataset and performs basic data analytics using Pandas.

import pandas as pd

# Step 1: Create a sample dataset
data = {
    "Name": ["Arun", "Bala", "Cathy", "David", "Elena"],
    "Age": [20, 21, 20, None, 22],
    "Department": ["ECE", "CSE", "ECE", "EEE", "CSE"],
    "Marks": [85, 90, None, 75, 88],
    "Attendance": [90.5, 95.0, 88.5, 80.0, None]
}

df = pd.DataFrame(data)

# Step 2: Display the dataset
print("Dataset:")
print(df)

# Step 3: Display the first five rows
print("\nFirst Five Rows:")
print(df.head())

# Step 4: Display dataset dimensions
print("\nDataset Shape:")
print(df.shape)

# Step 5: Display information about the dataset
print("\nDataset Information:")
df.info()

# Step 6: Display statistical summary
print("\nStatistical Summary:")
print(df.describe())

# Step 7: Check missing values
print("\nMissing Values:")
print(df.isnull().sum())

# Step 8: Check duplicate rows
print("\nDuplicate Rows:")
print(df.duplicated().sum())

# Step 9: Fill missing numerical values
df["Age"] = df["Age"].fillna(df["Age"].mean())
df["Marks"] = df["Marks"].fillna(df["Marks"].mean())
df["Attendance"] = df["Attendance"].fillna(
    df["Attendance"].mean()
)

# Step 10: Display cleaned dataset
print("\nCleaned Dataset:")
print(df)

# DATA PREPARATION FOR MACHINE LEARNING

After analyzing and cleaning the dataset, it can be prepared for Machine Learning.

Steps Involved

Handle missing values.

Remove duplicate records.

Identify input features and target variables.

Convert categorical data into numerical form when required.

Scale numerical features when appropriate.

Split the dataset into training and testing sets.

Example:

Input features: Age, Marks, and Attendance.

Target variable: Student performance category.

# APPLICATIONS

Student performance analysis.

Healthcare data analysis.

Business and customer analytics.

Financial data analysis.

Data preparation for Machine Learning.

Exploratory Data Analysis (EDA).


# RESULT
Data analytics was performed successfully on a sample dataset using Python and Pandas. The dataset structure, dimensions, data types, statistical information, missing values, and duplicate records were examined. Missing numerical values were handled using column means, and the dataset was prepared for further analysis and Machine Learning applications.
