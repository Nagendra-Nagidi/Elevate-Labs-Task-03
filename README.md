# Elevate-Labs-Task-03

In the above Taskfolder you can find all the necessary files regarding Task 3. In the Jupyter file 'task3_solutions.ipynb', I have implemented Linear Regression on Housing Dataset and created linear model to predict house prices. I have mainly used pandas,matplotlib to complete data preprocessing and visulisation and mainly dependent on the scikit learn library in python for creating the Linear Regression model in the following manner:

#### 1.Data Preprocessing
Encoded categorical variables (binary features using label encoding)
Applied one-hot encoding to furnishing status categories
Normalized numerical features:
RobustScaler for area (handles outliers)
MinMaxScaler for bedrooms, bathrooms, stories, and parking (preserves ordinal relationships)

#### 2.Model Training
Split data into 80% training and 20% testing sets
used Linear Regression class from sklearn.linear_model to implement Regression
Trained a multiple linear regression model to learn price relationships

#### 4.Evaluation Metrics:
evaluated model using mae,mse,r2 with the help of scikitlearn
Mean Absolute Error (MAE): ₹970,043.40
Mean Squared Error (MSE): ₹1,754,318,687,330.67
Root Mean Squared Error (RMSE): ₹1,324,506.96
R² Score: 0.6529 (65.29% of price variation explained)

#### 5.Key Visualizations for Model Interpretation
Actual vs. Predicted Prices Plot:
Created scatter plot comparing model predictions against true values
Added ideal fit line (y=x) to highlight perfect predictions
Visualized systematic errors through point dispersion patterns
Identified model bias: Underprediction of high-value properties
Feature Coefficient Analysis:
Generated sorted coefficient table highlighting dominant price drivers
Visual interpretation of feature impacts:
Area: Strong positive correlation (₹1.25M per unit)
Bathrooms: High incremental value (₹820K per unit)
Negative coefficients flagged for investigation (e.g., AC effect)
