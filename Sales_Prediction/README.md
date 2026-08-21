# Sales Prediction with Python

## Project Overview

The Sales Prediction with Python project uses the Advertising dataset to understand how advertising expenditure across different channels affects product sales.

The project applies Linear Regression to predict Sales based on advertising expenditure and compares Simple Linear Regression with Multiple Linear Regression.

The main objective of this project is to understand the relationship between advertising channels and sales and to evaluate how well Linear Regression can predict sales.

---

## Dataset

The project uses the Advertising dataset.

The dataset contains:

- 200 observations
- 4 columns

The columns are:

- TV
- Radio
- Newspaper
- Sales

`TV`, `Radio`, and `Newspaper` represent advertising expenditure, while `Sales` represents the resulting sales.

---

## Project Workflow

The project follows these steps:

1. Load the dataset
2. Describe and inspect the data
3. Check data types and missing values
4. Perform exploratory data analysis
5. Create histograms
6. Create boxplots
7. Create scatter plots
8. Analyze the correlation matrix
9. Create a pair plot
10. Build Simple Linear Regression
11. Build Multiple Linear Regression
12. Evaluate both models
13. Compare R², MAE, and RMSE
14. Analyze model residuals
15. Check regression assumptions
16. Interpret the regression coefficients
17. Draw business-related conclusions

---

## Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the distribution and relationships between the variables.

The following visualizations were created:

- Histograms
- Boxplots
- Scatter plots
- Correlation matrix
- Pair plot

The analysis helped identify the relationship between advertising expenditure and Sales.

---

## Simple Linear Regression

A Simple Linear Regression model was created using **TV advertising expenditure alone** to predict Sales.

TV advertising provides a reasonably good prediction of Sales, but using TV alone leaves some variation in Sales unexplained.

This motivated the use of additional advertising variables.

---

## Multiple Linear Regression

A Multiple Linear Regression model was created using:

- TV
- Radio
- Newspaper

as predictors of Sales.

Adding Radio and Newspaper allows the model to consider multiple advertising channels simultaneously.

The Multiple Linear Regression model showed a significant improvement in R² compared with the Simple Linear Regression model.

---

## Model Evaluation

The models were evaluated using the following metrics:

### R²

R² measures the proportion of variance in Sales explained by the model.

A higher R² indicates that the model explains more of the variation in the target variable.

### MAE

Mean Absolute Error (MAE) measures the average absolute difference between the actual and predicted Sales values.

A lower MAE indicates better performance.

### RMSE

Root Mean Squared Error (RMSE) measures the square root of the average squared prediction errors.

A lower RMSE indicates better performance and gives more weight to larger errors.

---

## Model Comparison

Two Linear Regression approaches were compared:

| Model | Predictors |
|---|---|
| Simple Linear Regression | TV |
| Multiple Linear Regression | TV, Radio, Newspaper |

The Multiple Linear Regression model performed better than the Simple Linear Regression model because it uses additional information from the other advertising channels.

---

## Residual Analysis

Residual analysis was performed to evaluate the assumptions of the regression model.

The following aspects were considered:

- Normality of residuals
- Homoscedasticity
- Independence of residuals

The residuals were reasonably well-behaved, indicating that the regression model assumptions hold up reasonably well for this dataset.

---

## Interpretation

The regression coefficients were examined to understand the business impact of each advertising channel.

The analysis showed that:

- **TV** is the single most important predictor of Sales.
- **Radio** adds substantial predictive value when combined with TV.
- **Newspaper** contributes very little once TV and Radio are included in the model.

---

## Key Findings

- TV is the strongest individual predictor of Sales.
- Radio provides substantial additional predictive value.
- Newspaper contributes relatively little after accounting for TV and Radio.
- Multiple Linear Regression explains a large share of the variation in Sales.
- The residuals are reasonably well-behaved.
- The regression model provides useful information for understanding the relationship between advertising expenditure and Sales.

---

## Business Insight

From a business perspective, a marketing team using this dataset would likely want to prioritize **TV and Radio advertising budgets**.

The analysis suggests that Newspaper advertising contributes relatively little to predicting Sales once TV and Radio spending are taken into account.

Therefore, the business could reconsider how much of its advertising budget should be allocated to Newspaper compared with TV and Radio.

---

## Conclusion

This project demonstrated the complete workflow of using Linear Regression for sales prediction.

The Advertising dataset was first explored through data description and exploratory data analysis. Different visualizations were used to understand the distributions and relationships between advertising channels and Sales.

A Simple Linear Regression model using TV advertising alone provided a decent prediction of Sales. However, the Multiple Linear Regression model using TV, Radio, and Newspaper provided a significant improvement in R².

The model was further evaluated using R², MAE, and RMSE, while residual analysis was used to check the assumptions of Linear Regression.

The analysis showed that **TV is the most important individual predictor**, while **Radio provides substantial additional value**. In contrast, **Newspaper contributes very little once TV and Radio are accounted for**.

Overall, the project demonstrates how regression analysis can be used not only to predict Sales but also to understand the business impact of different advertising channels.