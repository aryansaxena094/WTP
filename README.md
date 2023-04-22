# Water Treatment Plant

This project analyzes water quality data using various data preprocessing and machine learning techniques.

## Table of Contents
- [Contributors](#contributors)
- [Pre-processing](#pre-processing)
- [Finding Relationships](#finding-relationships)
- [Decision Tree Regressor](#decision-tree-regressor)
- [Classification](#classification)
- [Conclusion](#conclusion)

## Contributors
The contributors to this project are:
- Aryan Saxena
- Dina Omidvar
- Niloofar
- Rohan

## Pre-processing
The pre-processing stage involves handling missing values, removing columns with only NaN values, converting column values from strings to floats, and merging common columns from each year into a new data frame.

## Finding Relationships
In this stage, we identify strong correlations between features in the new data frame through pairwise feature comparison and correlation analysis. We also visualize these correlations through scatter plots.

## Decision Tree Regressor
We use a decision tree regressor to predict feature values. This involves selecting relevant features and the target variable, splitting the data into training and testing sets, training the model, measuring its accuracy using mean squared error, and computing its score on the training and testing sets. We also use hyperparameters to avoid overfitting.

## Classification
In this stage, we define the target variable as the healthiness of each water sample and create a new column called "Health Status" based on a threshold. We then classify water samples as healthy or unhealthy based on quality indicators detected by WHO such as pH, free chlorine, turbidity, and conductivity. We train and test various classification models including random forest classifier, SVM, logistic regression, and KNN to evaluate their performance. We compute the accuracy score using the accuracy_score function and print a classification report that includes precision, recall, and F1 score for each class. We also compute the confusion matrix using the confusion_matrix function to evaluate the model's performance.

## Conclusion
Pre-processing of data is a critical step in our analysis. Finding correlations between features is very important for making accurate predictions. We found a perfect correlation between TDS and conductivity. The random forest classifier gave us the highest accuracy for classification.