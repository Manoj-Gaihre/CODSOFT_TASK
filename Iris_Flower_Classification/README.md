# Iris Flower Classification

## Project Overview

The Iris Flower Classification project uses the Iris dataset to develop machine learning models that classify flowers into three different species based on their sepal and petal measurements.

The three species are:

- Iris-setosa
- Iris-versicolor
- Iris-virginica

The main objective of this project is to understand the complete classification workflow, from data exploration and visualization to model training, evaluation, cross-validation, and model tuning.

## Accuracy

#### Manual Classification

A manual classification function was created using the petal_length feature and predefined conditions to classify the Iris species.

The manual classification achieved:

Accuracy: 94.74%

This result shows that petal length alone provides a strong indication of the Iris species.

#### Machine Learning Models

Different machine learning classification models were trained and evaluated using the test dataset.

Logistic Regression:	94.74%
Random Forest:	92.11%
Decision Tree:	89.47%
K-Nearest Neighbors (KNN):	97.37%

## Best Test Accuracy

Among the machine learning models, K-Nearest Neighbors (KNN) achieved the highest test accuracy.

KNN Test Accuracy: 97.37%

Although KNN achieved the highest accuracy on the selected test set, a single train-test split may not always provide the most reliable estimate of model performance.

Therefore, cross-validation was also performed to compare the models more reliably.

## Cross Validation

Five-fold cross-validation was used to evaluate the models on different subsets of the training data.

Cross-validation helps determine how consistently a model performs instead of depending only on one train-test split.

The cross-validation accuracies were:

Logistic Regression:	96.40%
KNN:	95.49%
Random Forest:	93.75%
Decision Tree:	92.92%

## Cross Validation Best Accuracy

The Logistic Regression model achieved the highest cross-validation accuracy.

Best Cross-Validation Accuracy: 96.40%

Therefore, Logistic Regression was selected as the final model because it provided the best average performance across the five cross-validation folds.

The final Logistic Regression model used:
```
LogisticRegression(
    C=1,
    max_iter=200
)
```
Cross-validation was used for model selection rather than selecting the model only from the accuracy of one particular train-test split.

## Final Test Accuracy

After selecting Logistic Regression based on its best cross-validation performance, the final model was evaluated on the unseen test dataset.

Final Model: Logistic Regression

Final Test Accuracy: 94.74%

Cross-Validation Accuracy: 96.40%

The final model therefore achieved:

96.40% average accuracy during five-fold cross-validation.
94.74% accuracy on the unseen test dataset.

## Project Sturcture

```text
Iris_Flower_Classification/
│
├── data/
│   └── IRIS.csv
│
├── iris.ipynb
│
├── iris-project/
│   └── Python virtual environment
│
└── README.md
```

## Dataset

The project uses the `IRIS.csv` dataset located inside the `data` folder.

The dataset contains the following features:

- `sepal_length`
- `sepal_width`
- `petal_length`
- `petal_width`
- `species`

The target variable is:

```text
species
```

## Conclusion
In conclusion, we achieved a 94.74% accuracy on the test data set using a logistic regression model with these model parameters:
```
Logistic regression(C = 1, max_iter = 200)
```