# Titanic Dataset: Data Preprocessing, Cleaning, and Modeling

## Overview
This project is a complete data science workflow on the famous Titanic dataset. It covers all the essential steps from initial data exploration and cleaning to building and evaluating machine learning models. The primary goal is to predict passenger survival based on various features and to understand which factors were most influential in the outcome.

The Jupyter Notebook, `Titanic_Dataset_assignment.ipynb`, contains the complete code for this analysis.

## Project Steps
The project is structured into the following key phases:

### 1. Initial Data Exploration (EDA)
- **Loading Data**: Loading the `train.csv` file.  
- **Data Overview**: Using `df.info()` and `df.describe()` to examine data types, missing values, and statistical summaries.  
- **Visualization**: Visualizing the distributions of key features like `Survived`, `Age`, `Sex`, and `Pclass` to find initial insights.

### 2. Data Preprocessing and Cleaning
- **Handling Missing Values**:  
  - Missing `Age` values are filled with the median.  
  - `Embarked` values are filled with the mode.  
  - `Cabin` column is dropped due to excessive missing data.  
- **Feature Engineering**: A new feature, `FamilySize`, is created by combining `SibSp` and `Parch` to analyze the impact of family on survival.  
- **Encoding Categorical Features**:  
  - `Sex` column is converted to numerical values using `LabelEncoder`.  
  - `Embarked` column is one-hot encoded.  
- **Scaling Numerical Features**: `Age` and `Fare` are scaled using `StandardScaler` to ensure all features have a similar range.

### 3. Model Training and Evaluation
- **Data Splitting**: The cleaned dataset is split into training and testing sets.  
- **Model Selection**: Decision Tree and Logistic Regression models are used as baseline and slightly more complex alternatives.  
- **Cross-Validation**: K-Fold cross-validation (5 folds) is applied to get a robust estimate of model performance.  
- **Evaluation Metrics**: Accuracy, Precision, Recall, and F1-Score are calculated for model evaluation.

## How to Run the Notebook
1. **Download the Dataset**: Download the `train.csv` file from the Kaggle Titanic competition page.  
2. **Upload to Colab**: Upload the `train.csv` file to your Google Colab notebook's file system.  
3. **Run All Cells**: Open `Titanic_Dataset_assignment.ipynb` and run all code cells sequentially.

## Results Summary
The model evaluation using 5-Fold Cross-Validation provides a robust measure of performance.  

**Decision Tree Model Average Scores**:
- Accuracy: 0.7801  
- Precision: 0.7200  
- Recall: 0.6988  
- F1-Score: 0.7086

Edited by Ramdular Yadav
