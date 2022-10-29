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
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Meiyarasi.V
RegisterNumber: 212221230058


# LEAST SQUARE METHOD
import numpy as np
import matplotlib.pyplot as plt
X=np.array([0,1,2,3,4,5,6,7,8,9])
Y=np.array([1,3,2,5,7,8,8,9,10,12])
X_mean=np.mean(X)
print(X_mean)
Y_mean=np.mean(Y)
print(Y_mean)
num=0
denum=0
for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denum+=(X[i]-X_mean)**2
m=num/denum
print(m)
b=Y_mean - m*X_mean
print(b)
Y_pred=m*X+b
print(Y_pred)
plt.scatter(X,Y,color='purple')
plt.plot(X,Y_pred,color='red') 
plt.show() 

```

## Output:
![WhatsApp Image 2022-10-29 at 2 51 49 PM](https://user-images.githubusercontent.com/94748389/198824100-aa16e2d2-6869-4c0e-b327-39c603956707.jpeg)
![WhatsApp Image 2022-10-29 at 2 51 49 PM (1)](https://user-images.githubusercontent.com/94748389/198824112-b5122fd7-a73c-494f-8ad9-f44fdd42d334.jpeg)
![WhatsApp Image 2022-10-29 at 2 51 49 PM (5)](https://user-images.githubusercontent.com/94748389/198824279-01e1ac46-e353-4635-a44c-bbfef3972027.jpeg)
![WhatsApp Image 2022-10-29 at 2 51 49 PM (3)](https://user-images.githubusercontent.com/94748389/198824264-42647282-bd83-4fab-97ee-53a54d64b1c4.jpeg)
![WhatsApp Image 2022-10-29 at 2 51 49 PM (2)](https://user-images.githubusercontent.com/94748389/198824130-0d8d30b0-d4fd-4401-bf5b-384b8d844f4d.jpeg)
![WhatsApp Image 2022-10-29 at 2 51 49 PM (3)](https://user-images.githubusercontent.com/94748389/198824134-78124322-1655-426e-b07e-29274073ff6d.jpeg)



## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
