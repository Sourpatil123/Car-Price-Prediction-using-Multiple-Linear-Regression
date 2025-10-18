# Car-Price-Prediction-using-Multiple-Linear-Regression

📘 Project Overview

This project predicts car prices based on various features such as Age, KM, Fuel Type, HP, Automatic, cc, Doors, Cylinders, Gears, and Weight using a Multiple Linear Regression (MLR) model.

The goal is to analyze how each feature influences the Price and to build a regression model capable of predicting the car's value with high accuracy.

🎯 Objective

To develop a Multiple Linear Regression model that accurately predicts the Price of a car based on multiple independent variables, achieving a strong Train R² = 0.86 and Test R² = 0.86.

🧩 Dataset Overview
Feature	Description
Age	Age of the car (in years)
KM	Kilometers driven
Fuel_Type	Type of fuel (Petrol, Diesel, CNG, etc.)
HP	Horsepower of the car
Automatic	1 = Automatic, 0 = Manual
cc	Engine capacity (in cubic centimeters)
Doors	Number of doors
Cylinders	Number of cylinders in the engine
Gears	Number of gears
Weight	Weight of the car (in kg)

🎯 Target Variable:

Price – The car’s market value (in ₹ or chosen currency)

🧮 Model Used

Multiple Linear Regression (MLR) is applied to establish a linear relationship between multiple independent variables and the dependent variable (Price).

🧰 Technologies Used

Python 3.x 🐍

NumPy, Pandas – Data handling

Matplotlib, Seaborn – Visualization

Scikit-learn – Model creation and evaluation

SciPy, Statsmodels – Statistical validation

⚙️ Steps Followed
1️⃣ Data Preprocessing

Checked for missing/null values

Encoded categorical variables (Fuel_Type)

Removed duplicates and outliers

Split data into 80% Train and 20% Test

2️⃣ Exploratory Data Analysis (EDA)

Generated Heatmap to visualize correlation among features

Created Distribution Plots for all features

Used Pairplots to understand feature relationships

3️⃣ Model Building

Built a Multiple Linear Regression model using LinearRegression() from Scikit-learn

Trained on 80% data, tested on remaining 20%

4️⃣ Model Evaluation
Metric	Score
Train R² Score	0.86
Test R² Score	0.86
MSE	Low
MAE	Low
RMSE	Low

✅ The model performed consistently on both train and test data, indicating no overfitting.

📊 Visualizations & Statistical Checks
🔥 1. Correlation Heatmap

Helps visualize which features are most correlated with Price

Example: HP, cc, and Weight showed strong positive correlation

Age and KM showed negative correlation

📈 2. Probability Plot (Normality Check)

Used scipy.stats.probplot() to verify normal distribution of residuals

Residuals followed a linear pattern, confirming normality assumption

📉 3. Homoscedasticity Check (Residual vs Fitted Plot)

Ensures that residuals have constant variance across predicted values

A random scatter (no pattern) confirms Homoscedasticity

📊 4. Distribution Plot (Residuals)

Checked how residuals are distributed using Seaborn’s distplot()

💡 Key Insights

Age and KM negatively impact car price.

Horsepower, cc, and Weight have strong positive relationships with Price.

Automatic cars tend to cost more.

The model achieves balanced performance (Train/Test R² both 0.86).

🧾 Conclusion

The Multiple Linear Regression model effectively predicts car prices with high accuracy (R² = 0.86 on both train and test sets).
All linear regression assumptions — Linearity, Normality, Homoscedasticity, and Independence of Errors — were successfully validated.
