# linearreg
# Linear Regression Analysis on USA Housing Data

This repository contains Python code for performing linear regression analysis on the "USA_Housing.csv" dataset. The dataset consists of housing-related information such as average area income, house age, number of rooms, number of bedrooms, population, and prices of houses in the USA.

## Overview

The provided Python script conducts various analyses on the dataset using the `pandas`, `numpy`, `matplotlib`, and `seaborn` libraries. It performs the following tasks:

1. Loads the dataset using `pandas`.
2. Displays the first few rows of the dataset using `df.head()`.
3. Provides information about the dataset using `df.info()`.
4. Generates descriptive statistics using `df.describe()`.
5. Creates a pairplot to visualize the relationships between different variables using `sns.pairplot(df)`.
6. Plots a distribution plot for the 'Price' column using `sns.distplot(df["Price"])`.
7. Generates a heatmap to visualize the correlation matrix using `sns.heatmap(df.corr(), annot=True)`.

After the exploratory data analysis, the script proceeds with building a linear regression model to predict house prices based on the given features. It does the following:

1. Defines the feature matrix `X` and target variable `y`.
2. Splits the dataset into training and testing sets using `train_test_split` from `sklearn.model_selection`.
3. Instantiates a linear regression model using `LinearRegression()` from `sklearn.linear_model`.
4. Fits the model to the training data using `lm.fit(X_train, y_train)`.
5. Prints the intercept and coefficients of the linear regression model using `lm.intercept_` and `lm.coef_`.
6. Displays the names of the features using `X_train.columns`.

## Prerequisites

Make sure you have the following libraries installed:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn (for `train_test_split` and `LinearRegression`)

## Usage

1. Ensure that you have the "USA_Housing.csv" file in the same directory as the Python script.
2. Execute the Python script.
3. View the generated plots and printed information to analyze the dataset and linear regression model.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or feedback, please contact the repository owner:
- Name:kavipriya
- Email:kavipriyapanneerselvam22@gmail.com
