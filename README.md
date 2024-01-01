# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>
Get the independent variable X and dependent variable Y.

### Step2
<br>
Calculate the mean of the X -values and the mean of the Y -values.

### Step3
<br>
Find the slope m of the line of best fit. 

### Step4
<br>Use the slope m and the y -intercept to form the equation of the line.
### Step5
<br>
Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
#program to implement multivariate linear regression 
#developed by : dharshan pt
#register no:23005803
import pandas as ps
from sklearn import linear_model
data=ps.read_csv("cars.csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predict=regr.predict([[3300,1300]]) 
print('Predicted CO2 for for the corresponding weight and volume',predict)
```
## Output:
![image](https://github.com/etjabajasphin/Multivariate-Linear-Regression/assets/138849376/d1695aad-2bdb-43dd-b813-7e5096e5c429)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
