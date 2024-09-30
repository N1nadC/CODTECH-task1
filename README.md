# CODTECH-task1
Name: Ninad chaudhari
Company: CODTECH IT SOLUTIONS
Intern ID: CT08DS7778
Domain: ML
Overview
This project focuses on predicting housing prices using linear regression, one of the fundamental algorithms in machine learning. The project utilizes the California Housing dataset, a real-world dataset that includes various housing-related features like the number of rooms, number of bedrooms, housing age, and proximity to the ocean. The primary goal is to predict the median house value based on these features.

1. Dataset Overview
The California Housing dataset contains information about housing prices and related attributes in various districts of California. The dataset includes the following features:

total_rooms: The total number of rooms in a district.
total_bedrooms: The total number of bedrooms in a district.
housing_median_age: The median age of houses in a district.
ocean_proximity: Categorical feature that indicates how close the district is to the ocean.
median_house_value: The target variable, which represents the median value of houses in a district (in US dollars).
Data source: The dataset is publicly available and can be downloaded from here.

2. Project Objectives
The project’s objective is to:

Build a linear regression model to predict housing prices based on selected features.
Handle missing values and preprocess the data appropriately for model training.
Evaluate the model using various metrics to ensure accuracy and reliability.
3. Data Preprocessing
Before training the model, several preprocessing steps are necessary:

Handling Missing Values: Missing data in numeric columns (e.g., total_rooms and total_bedrooms) is imputed using the median of the column. For categorical columns (like ocean_proximity), the most frequent category is used to fill in missing values.
Feature Selection: The features used for prediction include total_rooms, total_bedrooms, housing_median_age, and ocean_proximity.
One-Hot Encoding: The ocean_proximity feature is categorical and needs to be converted into numerical values using one-hot encoding.
Scaling: Numeric features are scaled using StandardScaler to normalize the data, making the training process more efficient.
4. Modeling with Linear Regression
Linear Regression is a simple yet effective algorithm for predicting continuous outcomes. It models the relationship between input features (independent variables) and the target variable (dependent variable) by fitting a linear equation to the data.
The linear regression model is trained on 80% of the dataset, with 20% of the data held out for testing.
5. Evaluation Metrics
Once the model is trained, it is evaluated using the following metrics:

Mean Absolute Error (MAE): Measures the average magnitude of the errors in a set of predictions, without considering their direction.
Mean Squared Error (MSE): Measures the average squared difference between the estimated values and the actual value.
R² Score: Represents the proportion of the variance for the target variable that’s explained by the model.
6. Making Predictions
After evaluating the model, predictions can be made on new data. The model is tested by predicting the median house value based on new inputs for total_rooms, total_bedrooms, housing_median_age, and ocean_proximity.

7. Conclusion
This project demonstrates the application of a linear regression model to predict housing prices. While linear regression offers a good starting point, further enhancements could be made by exploring more advanced regression techniques, conducting hyperparameter tuning, or engineering additional features to improve the accuracy of the predictions.
