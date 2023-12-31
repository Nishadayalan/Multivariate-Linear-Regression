# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import Pandas library.

### Step2
Import Linear_model from sklearn.

### Step3
Read the csv file using pandas library.

### Step4
Enter the parameters of the linear function.


### Step5
Print the parameters of the linear function.


## Program:
```
#Developed by:NISHA.D
#Register number:212223230143
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("cars.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
print('Amount:',regr.predict([[3300,1300]]))

```
## Output:

### Insert your output

![Alt text](<Screenshot 2023-12-31 144348.png>)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.