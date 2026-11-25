# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Import pandas and linear_model from sklearn.



### Step2
<br>Load the dataset from "carsemission.csv" into a DataFrame.


### Step3
<br>Assign 'Weight' and 'Volume' as features (
𝑋
X) and 'CO2' as the target (
𝑦
y).




### Step4
<br>Initialize the LinearRegression model and fit it with 
𝑋
X and 
𝑦
y.


### Step5
<br>Print the model coefficients and intercept.

### Step6
<br>Provide new input data (Weight: 3300, Volume: 1300) to predict and print the expected CO2 emissions.


## Program:
```
Developed by: Yuvethika V
Register no: 26016105
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)

```
## Output:


<br><img width="938" height="455" alt="image" src="https://github.com/user-attachments/assets/0c8a6f77-d883-4463-9256-7e439f006de7" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
