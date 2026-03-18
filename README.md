# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1: Import the required libraries such as Pandas and Scikit-learn to handle data and perform linear regression.

### Step2: Read the cars.csv file using Pandas and store it in a dataframe.

### Step3: Select Weight and Volume as independent variables (X) and CO2 as the dependent variable (y).


### Step4: Create a linear regression model and train it using the dataset with the fit() function.


### Step5: Then use the trained model to predict the CO2 emission and display the result.

## Program:
```
Developed by: Sadhana R
Register No: 212225240129
```
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))
```
## Output:
![alt text](<Screenshot 2026-03-18 143857.png>)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.