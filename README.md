# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 1. Load the dataset into a DataFrame and explore its contents to understand the data
structure.
2.Separate the dataset into independent (X) and dependent (Y) variables, and split them
into training and testing sets.
3.Create a linear regression model and fit it using the training data.
4.Predict the results for the testing set and plot the training and testing sets with fitted
lines.
5.Calculate error metrics (MSE, MAE, RMSE) to evaluate the model’s performance.

 
 

## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by:S.Kowshik Ram
RegisterNumber:212225230143
import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

# Sample data

X = np.array([1, 2, 3, 4, 5]).reshape(-1, 1)
Y = np.array([35, 50, 65, 70, 85])

# Create model
model = LinearRegression()

# Train model
model.fit(X, Y)

# Get slope and intercept
m = model.coef_[0]
b = model.intercept_

print("Slope (m):", m)
print("Intercept (b):", b)

# ---- Prediction ----
x_input = float(input("Enter hours studied: "))
predicted_marks = model.predict([[x_input]])
print("Predicted Marks:", predicted_marks[0])

# ---- Plot ----
Y_pred = model.predict(X)

plt.scatter(X, Y, label="Actual Data")
plt.plot(X, Y_pred, label="Regression Line")
plt.xlabel("Hours Studied")
plt.ylabel("Marks Scored")
plt.title("Simple Linear Regression (Using sklearn)")
plt.legend()
plt.show()
  
*/
```

## Output:
<img width="858" height="681" alt="Screenshot 2026-04-21 111357" src="https://github.com/user-attachments/assets/bdeef469-2935-4c56-9a08-c8eee5f1148e" />



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
