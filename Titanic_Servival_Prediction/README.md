# Titanic Survival Prediction

## Project Overview

The Titanic Survival Prediction project is a beginner-level machine learning classification project. The goal is to build a model that predicts whether a passenger on the Titanic survived or did not survive based on passenger information.

This project covers the complete machine learning workflow, including data loading, data cleaning, exploratory data analysis, preprocessing, model training, and model evaluation.

## Objective

The main objective of this project is to develop a machine learning model that predicts whether a Titanic passenger survived.

### Target Variable

- `0` → Did not survive
- `1` → Survived

## Dataset

The Titanic dataset contains information about individual passengers.

Important features include:

- `PassengerId`
- `Pclass`
- `Name`
- `Sex`
- `Age`
- `SibSp`
- `Parch`
- `Ticket`
- `Fare`
- `Cabin`
- `Embarked`
- `Survived`

## Technologies Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Project Workflow

1. Load the dataset
2. Understand the dataset
3. Check for missing values
4. Clean the data
5. Perform Exploratory Data Analysis (EDA)
6. Visualize important relationships
7. Select and preprocess features
8. Split the data into training and testing sets
9. Train machine learning models
10. Evaluate the models
11. Compare model performance
12. Select the best-performing model

## Data Preprocessing

The following preprocessing steps were performed:

- Checked the structure and information of the dataset
- Identified missing values
- Handled missing values
- Selected relevant features
- Encoded categorical variables
- Prepared the dataset for machine learning

## Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the relationship between passenger characteristics and survival.

The analysis included:

- Survival distribution
- Survival by gender
- Survival by passenger class
- Age distribution
- Fare distribution
- Feature relationships and correlations

Visualizations were created using Matplotlib and Seaborn.

## Machine Learning Models

Two classification models were trained and compared.

### Logistic Regression

Logistic Regression was used as a baseline classification model for predicting whether a passenger survived.

### Random Forest Classifier

Random Forest was used as an ensemble learning model to capture more complex relationships between the features.

## Model Results

| Model | Accuracy |
|---|---:|
| Logistic Regression | 80% |
| Random Forest | 82% |

## Best Model

The Random Forest Classifier performed better than Logistic Regression based on accuracy.

- Logistic Regression: **80%**
- Random Forest: **82%**

Therefore, Random Forest was selected as the better-performing model in this project.

## What I Learned

Through this project, I learned:

- How to load and inspect a dataset using Pandas
- How to identify and handle missing values
- How to perform exploratory data analysis
- How to visualize data using Matplotlib and Seaborn
- How to preprocess categorical data
- How to split data into training and testing sets
- How to train classification models using Scikit-learn
- How to compare machine learning models
- How to evaluate model performance using accuracy

## Challenges Faced

- Handling missing values in the dataset
- Selecting useful features for prediction
- Encoding categorical variables
- Understanding different classification algorithms
- Comparing model performance
- Selecting the best-performing model

## Project Structure

```text
Titanic_Survival_Prediction/
│
├── Titanic_Survival_Prediction.ipynb
├── README.md
├── data/
│   └── Titanic.csv
```