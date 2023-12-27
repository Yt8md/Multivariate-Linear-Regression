# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1

import pandas as pd.
<br>

### Step2

Read the csv file.
<br>

### Step3

Get the value of X and y variables
<br>

### Step4
Create the linear regression model and fit.
<br>

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.
<br>

## Program:
```

## Developed by: Mathesh S
## Reg no: 23013902

import pandas as pd
from sklearn import linear_model
df=pd.read_csv('/boot/cars (1) (1).csv')
a=df[["Weight","Volume"]]
b=df[["CO2"]]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))

```
## Output:

![Alt text](image.png)


<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.