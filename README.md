<img width="1228" height="652" alt="Screenshot 2025-10-17 152454" src="https://github.com/user-attachments/assets/a568c249-44e7-4002-bcf4-9ba9d64bf034" /># Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

## Step 1

Load the dataset using pandas.


## Step 2

Select input features (Weight, Volume) and target variable (CO2).

## Step 3

Create and train the Linear Regression model using the selected data.

## Step 4

Display the model’s coefficients and intercept.


## Step 5

Predict CO2 emission for given input values (3300, 1300).

## Program:
```
import pandas as pd

from sklearn import linear_model

df=pd.read_csv("C:\\Users\\admin\\Downloads\\car (1).csv")

df

x=df[['Weight', 'Volume']]

y=df['CO2']

regr=linear_model.LinearRegression()

regr.fit(x,y)

print('Coefficients: ',regr.coef_)

print('Intercept:',regr.intercept_)

predictedCO2=regr.predict([[3300,1300]])

print("Predicted:",predictedCO2)


```
## Output

<img width="1228" height="652" alt="Screenshot 2025-10-17 152454" src="https://github.com/user-attachments/assets/6fa801bf-e51f-4b57-a7be-185bdc89ea07" />





## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
