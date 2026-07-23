# Car Price Prediction with Machine Learning

A regression project that predicts a used car's selling price based on its features, using machine learning.

This project was completed as **Task 3** for the **CodeAlpha Data Science Internship**.

## Overview

Using a dataset of used car listings, this project builds a model to predict a car's selling price based on features like present price, kilometers driven, age, fuel type, seller type, and transmission.

## Tools & Libraries

- Python
- Pandas
- Scikit-learn (`LinearRegression`, `train_test_split`, `mean_absolute_error`, `r2_score`)
- Matplotlib
- Seaborn

## Approach

1. Loaded and inspected the dataset
2. Feature engineering: converted `Year` into `Car_Age` (more directly useful for predicting price), and dropped `Car_Name` (too many unique values to be useful)
3. Converted categorical features (`Fuel_Type`, `Selling_type`, `Transmission`) into numeric form using one-hot encoding
4. Split the data into training (80%) and testing (20%) sets
5. Trained a Linear Regression model on the training data
6. Evaluated the model using Mean Absolute Error and R² Score
7. Visualized actual vs. predicted prices to assess model performance

## Results

- **Mean Absolute Error:** ~1.22 lakh
- **R² Score:** ~0.85 — the model explains about 85% of the variation in car prices

The actual vs. predicted price scatter plot shows most predictions clustering closely around the ideal prediction line, indicating strong model performance.

## How to Run

1. Open `Car_Price_Prediction.ipynb` in Google Colab or Jupyter Notebook
2. Upload the dataset CSV file when prompted
3. Run each cell in order to reproduce the preprocessing, training, and evaluation

## Author

Yukthika — CodeAlpha Data Science Intern
