

Overview

This project builds a Linear Regression model to predict housing prices based on numerical features. The dataset contains various attributes of houses, such as the number of bedrooms, square footage, and age. The project follows a structured workflow, including data preprocessing, model training, evaluation, and visualization.

Features Used

The dataset contains multiple features, but we focus on numerical attributes while ignoring categorical ones (like Address). The target variable is Price.

Project Workflow

1. Data Preprocessing

Selected numerical columns for X (features) and assigned Price to y (target variable).

Split data into training (70%) and testing (30%) sets using train_test_split().

2. Building the Linear Regression Model

Used sklearn.linear_model.LinearRegression() to fit the model on the training data.

Extracted the intercept and coefficients to analyze feature importance.

3. Making Predictions

Predicted housing prices using lm.predict(X_test).

Stored predictions in a NumPy array and compared them against actual values.

4. Model Evaluation

Calculated the following metrics:

Mean Absolute Error (MAE): Measures average absolute difference between actual and predicted values.

Mean Squared Error (MSE): Measures the squared average difference.

Root Mean Squared Error (RMSE): Provides an interpretable error measure in the same unit as Price.

R² Score: Evaluates the proportion of variance explained by the model.

5. Visualization

Scatter Plots: Explored relationships between individual features and Price.

Residual Histogram: Checked normality of residuals using sns.histplot() to validate model assumptions.

Installation & Requirements
pip install pandas numpy scikit-learn seaborn matplotlib

Results & Insights

The model provides insights into the impact of each feature on price predictions.

A well-distributed residual plot suggests that linear regression is a suitable model for this dataset.

Further improvements could include feature engineering or using non-linear models for better accuracy.

Future Improvements

Feature Scaling: Standardizing features to improve model performance.

Handling Outliers: Detecting and removing extreme values.

Exploring Other Models: Testing Decision Trees or Random Forest for better accuracy.
