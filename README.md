# Machine Learning Project: Decision Trees and Linear Regression Models

## Project Overview

This project demonstrates two fundamental machine learning models: **Decision Trees** and **Linear Regression**. We applied these models to real-world datasets to showcase their use in classification and prediction tasks, respectively. Visualizations and evaluations are provided to help interpret the model's performance.

## Table of Contents

1. [Project Objectives](#project-objectives)
2. [Dataset Information](#dataset-information)
3. [Models Used](#models-used)
    - [Decision Tree Classifier](#decision-tree-classifier)
    - [Linear Regression](#linear-regression)
4. [Model Working](#model-working)
    - [Decision Tree Model](#decision-tree-model)
    - [Linear Regression Model](#linear-regression-model)
5. [Visual Interpretations](#visual-interpretations)
6. [How to Run the Code](#how-to-run-the-code)
7. [Results](#results)
8. [Conclusion](#conclusion)

## Project Objectives

The goal of this project is to:
- Build a **Decision Tree Classifier** to classify iris species based on sepal and petal dimensions.
- Build a **Linear Regression Model** to predict house prices in California based on the number of rooms and house size.
- Evaluate both models using visualizations like confusion matrix, feature importance, residual plots, and scatter plots.
- Explain and interpret the visualizations to understand model performance and feature impact.

## Dataset Information

- **Iris Dataset**: A well-known dataset consisting of 150 samples of iris flowers with four features: sepal length, sepal width, petal length, and petal width. The target is the species of the flower (Setosa, Versicolor, or Virginica).
- **California Housing Dataset**: This dataset contains information on house prices in California, with features like median income, average number of rooms, average household size, etc.

## Models Used

### Decision Tree Classifier

- **Usage**: The Decision Tree is used to classify the iris species.
- **Method**: The tree is built by splitting the dataset on the feature that provides the most information gain at each step. The process continues until the data is categorized into a final class (species).
- **Evaluation**: Confusion matrix and decision tree structure help visualize how well the model performs and the decisions it makes at each node.

### Linear Regression

- **Usage**: The Linear Regression model is used to predict house prices based on the number of rooms and house size.
- **Method**: A linear relationship is established between the input features (number of rooms, house size) and the output (house price). The model fits a line to minimize the difference between actual and predicted values.
- **Evaluation**: Scatter plots and residual plots are used to visualize how well the predictions align with actual values and how errors are distributed.

## Model Working

### Decision Tree Model

1. **Data**: The Iris dataset with four features.
2. **Algorithm**: The Decision Tree Classifier splits data at each node based on feature values (e.g., petal length) to classify the flower species.
3. **Evaluation**: 
    - **Confusion Matrix**: Shows classification accuracy for each species.
    - **Feature Importance**: Highlights which features contribute most to classification decisions.
    - **Tree Visualization**: Shows the full decision-making process at each node.

### Linear Regression Model

1. **Data**: The California Housing dataset, using number of rooms and house size.
2. **Algorithm**: Linear Regression fits a line through the data to predict house prices based on the input features.
3. **Evaluation**:
    - **Scatter Plot**: Compares actual and predicted house prices.
    - **Residual Plot**: Shows the error distribution between predicted and actual values.
    - **Feature Importance**: Identifies how much each feature contributes to house price predictions.

## Visual Interpretations

- **Decision Tree Confusion Matrix**: Demonstrates perfect classification performance across all classes in the Iris dataset.
- **Decision Tree Feature Importance**: Shows that petal length and petal width are the most significant features for classification.
- **Linear Regression Scatter Plot**: Displays how close the predicted house prices are to the actual prices, with points ideally lying on the diagonal line.
- **Linear Regression Residual Plot**: Illustrates how well the model predicts by showing residuals around the zero line.

## How to Run the Code

1. Clone the repository.
2. Install the required Python packages:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the models in separate Python scripts:
    - **Decision Tree Model**:
      ```bash
      python decision_tree_iris.py
      ```
    - **Linear Regression Model**:
      ```bash
      python linear_regression_housing.py
      ```

## Results

- **Decision Tree Model**:
    - Achieved 100% accuracy in classifying iris species.
    - The decision tree structure highlights the decision points at each node, with petal length being the most significant feature.
  
- **Linear Regression Model**:
    - Predicted house prices with reasonable accuracy.
    - Feature importance shows that the number of rooms has the most influence on predicting house prices.

## Conclusion

This project demonstrates the application of **Decision Trees** for classification and **Linear Regression** for predicting continuous variables. By interpreting the results using confusion matrices, feature importance, and various plots, we gain insights into how the models perform and what factors influence their predictions.
