# EX 1-Implementation of Univariate Linear Regression
## DATE: 17.08.23
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
Developed by: DIVYA.A
RegisterNumber: 212222230034
X=np.array(eval(input()))
Y=np.array(eval(input()))
### Mean:

X_mean=np.mean(X)
print(X_mean)
Y_mean=np.mean(Y)
print(Y_mean)
num=0    # for slope
denum=0  # for slope

###  To find sum of(xi-x')&(yi-y')&(xi-x')^2:

for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denum+=(X[i]-X_mean)**2
m=num/denum
print(m)

### calculate intercept
b=Y_mean - m*X_mean
print(b)
### to plot graph
Y_pred=m*X+b
print(Y_pred)
plt.scatter(X,Y,color='blue')
plt.plot(X,Y_pred,color='yellow') 
plt.show() 
*/
```

## Output:
![EX 01](https://github.com/Divya110205/Find-the-best-fit-line-using-Least-Squares-Method/assets/119404855/08b0ca38-5d0f-48c6-b5e0-ae40c6cd902f)

## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
