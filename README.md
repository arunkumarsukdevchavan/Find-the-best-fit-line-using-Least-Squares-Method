# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
## Developed By: ARUN KUMAR SUKDEV CHAVAN
## Register No: 212222230013
```python
import numpy as np
import matplotlib.pyplot as plt
x=np.array(eval(input()))
y=np.array(eval(input()))
xmean=np.mean(x)
ymean=np.mean(y)
num=0
denom=0
for i in range(len(x)):
    num+=(x[i]-xmean)*(y[i]-ymean)
    denom+=(x[i]-xmean)**2
m=num/denom
c=ymean-m*xmean
print("slope",m)
print("Y-intercept",c)
ypred=m*x+c
print("Predicted values",ypred)
plt.scatter(x,y)
plt.plot(x,ypred)
plt.show()
```

## Output:
![Screenshot 2024-02-22 110601](https://github.com/r-sathish-02/Find-the-best-fit-line-using-Least-Squares-Method/assets/118787261/6d33473a-d139-47cc-89b7-bc2e26bdcbf5)



## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
