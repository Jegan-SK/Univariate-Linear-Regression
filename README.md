# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
import numpy as np
X=np.array(eval(input()))
Y=np.array(eval(input()))
X_mean=np.mean(X)
Y_mean=np.mean(Y)
n=d=0
for i in range(len(X)):
    n+=(X[i]-X_mean)*(Y[i]-Y_mean)
    d+=(X[i]-X_mean)**2
m=n/d
b=Y_mean-m*X_mean
print("Slope of the line,m=",m)
print("Y intercept of the line,b=",b)
Y_pred=m*X+b
print(Y_pred)





```
## Output
<img width="411" height="208" alt="Screenshot (64)" src="https://github.com/user-attachments/assets/0b8a02e6-ecb3-4b18-a4e9-f745d47252ac" />


## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
