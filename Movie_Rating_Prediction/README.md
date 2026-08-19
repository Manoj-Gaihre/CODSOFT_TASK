# 🎬 Movie Rating Prediction System

A Machine Learning regression project that predicts movie ratings based on features such as genre, director, and actors.

This project was developed as part of my Data Science and Machine Learning learning journey, with a focus on understanding the complete machine learning workflow — from data preprocessing and feature engineering to model training and evaluation.

---

## 📌 Project Overview

The goal of this project is to build a machine learning model that can predict the **rating of a movie** based on available movie-related information.

The project uses the **IMDb Movies India dataset**, which contains information about Indian movies, including:

- Movie Name
- Year
- Duration
- Genre
- Rating
- Votes
- Director
- Actor 1
- Actor 2
- Actor 3

The original dataset contains **15,509 rows and 10 columns**.

---

## 🎯 Objective

The main objective of this project is:

> **To build a regression model that predicts the rating of a movie based on features such as genre, director, and actors.**

This project also aims to compare different regression algorithms and determine which model performs best on the test dataset.

---

## 📂 Dataset

The dataset used in this project is:

**IMDb Movies India Dataset**

The dataset contains the following columns:

| Column | Description |
|---|---|
| `Name` | Name of the movie |
| `Year` | Release year of the movie |
| `Duration` | Duration of the movie |
| `Genre` | Genre or genres of the movie |
| `Rating` | Movie rating — target variable |
| `Votes` | Number of votes received |
| `Director` | Director of the movie |
| `Actor 1` | Main actor |
| `Actor 2` | Second actor |
| `Actor 3` | Third actor |

---

## 🔍 Exploratory Data Analysis

The dataset was first explored to understand its structure and identify missing values.

Missing values were found in several columns:

- Year
- Duration
- Genre
- Rating
- Votes
- Director
- Actor 1
- Actor 2
- Actor 3

The `Rating` column contains the target variable, so rows where the rating was missing were removed instead of filling the missing ratings with mean or median values.

---

## 🧹 Data Preprocessing

Several preprocessing steps were performed before training the machine learning models.

### 1. Handling Missing Target Values

Since this is a supervised regression problem, the model requires the actual target value during training.

Therefore, rows with missing `Rating` values were removed.

```python
df = df.dropna(subset=["Rating"])
```
--- 

### 2. Handling Missing Categorical Values

Missing values in categorical features such as:

- Genre
- Director
- Actor 1
- Actor 2
- Actor 3

were handled during preprocessing.

--- 


## ✂️ Train-Test Split

After preprocessing and feature engineering, the dataset was divided into:

- Training data
- Testing data

The training dataset was used to train the machine learning models, while the testing dataset was used to evaluate their performance on unseen data.

## 🤖 Machine Learning Models

Three regression algorithms were implemented and compared.

### 1. Linear Regression

Linear Regression was used as a baseline regression model.

LinearRegression()

### 2. Random Forest Regressor

A Random Forest Regressor was implemented using multiple decision trees.

### 3. Gradient Boosting Regressor

Gradient Boosting Regressor was also used to capture more complex relationships between the features and movie ratings.

## 📊 Model Evaluation

The performance of the regression models was evaluated using the following metrics:

### Mean Absolute Error (MAE)
Measures the average absolute difference between the actual and predicted movie ratings.

### Root Mean Squared Error (RMSE)
Measures the square root of the average squared prediction errors, giving more importance to larger errors.

### R² Score
Measures how well the model explains the variation in movie ratings. A higher R² score indicates better predictive performance.

---

## 📈 Model Performance

The following regression models were trained and evaluated:

| Model | MAE | RMSE | R² Score |
|---------|---------|---------|---------|
| Linear Regression | 1.0157 | 1.2685 | 0.1345 |
| Random Forest Regressor | 1.0046 | 1.2573 | 0.1496 |
| Gradient Boosting Regressor | **0.9773** | **1.2285** | **0.1883** |

### 🏆 Best Performing Model

**Gradient Boosting Regressor** achieved the best performance among all tested models with:

- **MAE:** 0.9773
- **RMSE:** 1.2285
- **R² Score:** 0.1883

The model produced the lowest prediction error and the highest R² score, making it the most effective model for predicting movie ratings in this project.

💡 Key Learnings

Through this project, I gained practical experience in:

- Data loading and exploration
- Exploratory Data Analysis
- Identifying and handling missing values
- Preparing a dataset for supervised learning
- Feature engineering
- Encoding categorical information
- Creating frequency-based features
- Train-test splitting
- Regression model implementation
- Model comparison
- MAE, RMSE, and R² evaluation
- Understanding the strengths and limitations of different regression algorithms

## 📌 Conclusion

This project successfully developed a machine learning regression system for predicting movie ratings using the IMDb Movies India dataset.

Three regression models—Linear Regression, Random Forest Regressor, and Gradient Boosting Regressor—were trained and evaluated. Based on the evaluation metrics, Gradient Boosting Regressor achieved the best overall performance.

The project provided valuable hands-on experience in data analysis, feature engineering, model training, and performance evaluation, strengthening my understanding of machine learning regression techniques.