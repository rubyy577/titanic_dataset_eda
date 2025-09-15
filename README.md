# Titanic Dataset: Data Preprocessing, Cleaning, and EDA

## Overview
This project is a data preprocessing and exploratory data analysis (EDA) assignment focused on the famous Titanic dataset, available on Kaggle. The goal is to clean the raw data, prepare it for machine learning, and perform a deep analysis to uncover patterns related to passenger survival.

The notebook performs the following key tasks:

- **Data Loading and Initial Exploration**: Loading the `train.csv` file and examining its structure, data types, and initial statistics.
- **Handling Missing Values**: Identifying and addressing missing data in key columns like `Age`, `Cabin`, and `Embarked`.
- **Feature Engineering**: Creating a new feature, `FamilySize`, to better understand the impact of family on survival.
- **Feature Encoding**: Converting categorical features (`Sex`, `Embarked`) into a numerical format suitable for modeling.
- **Feature Scaling**: Standardizing numerical features (`Age`, `Fare`) to a consistent scale.
- **Exploratory Data Analysis (EDA)**: Visualizing relationships between different features and the `Survived` target variable to gain insights.

## How to Run the Notebook
1. **Download the Dataset**: Download the `train.csv` file from the Kaggle Titanic competition page.
2. **Upload to Google Colab**: Upload the `train.csv` file directly to your Google Colab notebook's file system.
3. **Open the Notebook**: Open the `Titanic Dataset assignment.ipynb` notebook in Google Colab.
4. **Run All Cells**: Run all the code cells in the notebook in sequence. The code is structured to perform each step from loading to final analysis.

## Key Findings from EDA
Based on the analysis, several factors were highly correlated with a passenger's chance of survival:

- **Gender**: Females had a significantly higher survival rate than males, supporting the "women and children first" protocol.
- **Passenger Class**: Passengers in the first class had a much higher survival rate compared to those in the second and third classes, indicating that social status was a major factor.
- **Family Size**: Passengers traveling with small families (2-4 people) had the best survival rates. Those traveling alone or in very large families were less likely to survive.
- **Fare**: There was a strong positive correlation between the ticket fare and survival, which is likely related to passenger class.
