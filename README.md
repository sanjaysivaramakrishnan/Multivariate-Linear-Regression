# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1 : import pandas as numpy 
<br>

### Step2 : read the csv file using read_cas 
<br>

### Step3 : perform the requierd operation to slove hte problem
<br>

### Step4 : find hte coefficient and intercept 
<br>

### Step5 : finally print the value
<br>

## Program:
```
# Developed by: Sanjay sivaramakrishnan M
# RegisterNumber: 23013798

import pandas as pd
from sklearn import linear_model
df=pd.read_csv(r'C:\Users\admin\OneDrive\for python\py\maths.py\cars.csv')
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume",predictedCO2)

```
## Output:

### Insert your output
![image](https://github.com/sanjaysivaramakrishnan/Multivariate-Linear-Regression/assets/151629616/96557815-eb87-40d7-b70c-df521e7dbb1a)

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
