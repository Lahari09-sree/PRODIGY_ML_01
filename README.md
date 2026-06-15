# House Price Prediction Using Linear Regression

## Prodigy InfoTech Machine Learning Internship — Task 01

This project implements a multiple linear regression model to predict house prices based on:

* Above-ground living area in square feet
* Number of bedrooms
* Total number of bathrooms

## Dataset

The project uses the House Prices: Advanced Regression Techniques dataset from Kaggle.

Dataset link:
https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data

## Features Used

* `GrLivArea` — above-ground living area in square feet
* `BedroomAbvGr` — number of bedrooms above ground
* `TotalBathrooms` — combined number of full and half bathrooms

The total number of bathrooms was calculated using:

```python
TotalBathrooms = (
    FullBath
    + 0.5 * HalfBath
    + BsmtFullBath
    + 0.5 * BsmtHalfBath
)
```

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Google Colab

## Project Workflow

1. Loaded and explored the dataset.
2. Selected the required features.
3. Created the `TotalBathrooms` feature.
4. Split the data into training and testing sets.
5. Trained a Linear Regression model.
6. Predicted house prices using the test data.
7. Evaluated the model using MAE, RMSE and R² score.
8. Visualized actual prices against predicted prices.
9. Tested the model using custom house details.

## Model Evaluation

The model was evaluated using:

* Mean Absolute Error
* Root Mean Squared Error
* R² Score

Points closer to the diagonal line in the Actual vs Predicted Price graph represent more accurate predictions.

## Example Prediction

For a house with:

* 2,000 square feet
* 3 bedrooms
* 2.5 bathrooms

The predicted house price was approximately:

**$232,016.59**

## Project Files

* `PRODIGY_ML_01_House_Price_Prediction.ipynb` — complete project notebook
* `house_price_predictions.csv` — actual and predicted house prices
* `actual_vs_predicted.png` — model prediction visualization

## Conclusion

The Linear Regression model successfully predicted house prices using square footage, bedrooms and bathrooms. The project also demonstrated data preprocessing, feature engineering, model training, evaluation and visualization.

## Internship

This project was completed as Task 01 of the Machine Learning Internship at Prodigy InfoTech.

#ProdigyInfoTech

