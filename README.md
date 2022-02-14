# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Import panda



### Step2
<br>
Import linear model from sklearn

### Step3
<br>
Read the file using read_csv.


### Step4
<br>
Get the inputs from the user as x and y.



### Step5
<br>
Use regr.fit(x,y) to et the output.


## Program:
```
#DEVELOPED BY: M.RAJESHKANNAN
#REG NO: 21500434

import pandas as pd
from sklearn import linear_model

df =pd.read_csv("cars.csv")
x= df[["Weight","Volume"]]
y= df["CO2"]
regr =linear_model.LinearRegression()
regr.fit(x,y)

print("coefficients: ",regr.coef_)
print("Intercept: ",regr.intercept_)
predictedco2=regr.predict([[3000,1200]])
print("Predicted co2 for the coressponding weight and volume ",predictedco2)



```
## Output:

### Insert your output

![Op](https://user-images.githubusercontent.com/93901857/153826538-c3ab1095-980e-446b-9e68-ff56fc8b09f4.jpg)
<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.