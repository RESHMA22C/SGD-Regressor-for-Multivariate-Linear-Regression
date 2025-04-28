# SGD-Regressor-for-Multivariate-Linear-Regression

## AIM:
To write a program to predict the price of the house and number of occupants in the house with SGD regressor.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Load and Prepare Dataset Load California housing dataset using fetch_california_housing().
Convert the data to a DataFrame.

Add HousingPrice (target) as a new column.

2.Define Features (x) and Targets (y) Remove AveOccup and HousingPrice from features — keep them as targets.
So:

x = all features except AveOccup and HousingPrice

y = AveOccup and HousingPrice (multi-output regression)

3.Train-Test Split Split the data into 80% training and 20% testing using train_test_split().

4.Feature Scaling Use StandardScaler to normalize:

x_train and x_test (feature scaling)

y_train and y_test (target scaling — crucial for SGD)

5.Train Multi-Output Regressor Create SGDRegressor model for linear regression using stochastic gradient descent.
Wrap it in MultiOutputRegressor to handle multiple target variables.

Train the model using scaled x_train and y_train.

6.Make Predictions Predict on x_test, getting scaled predictions for both outputs.
Inverse transform the predictions and actual values using scaler_y to return to original scale.

7.Evaluate the Model Compute MSE between actual and predicted values (for both outputs).
Print the MSE and show the first 5 predictions.



## Program:
```
/*
Program to implement the multivariate linear regression model for predicting the price of the house and number of occupants in the house with SGD regressor.
Developed by: RESHMA C 
RegisterNumber:  212223040168
*/
```

## Output:
![image](https://github.com/user-attachments/assets/db1744cc-8252-4d71-b689-85bd9d2eef25)



## Result:
Thus the program to implement the multivariate linear regression model for predicting the price of the house and number of occupants in the house with SGD regressor is written and verified using python programming.
