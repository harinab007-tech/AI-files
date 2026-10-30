# Linear Regression Models in Machine Learning (Academic Tribe)
## Introduction
Linear Regression is a machine learning algorithm based on supervised learning. It performs a regression task. Regression models a target prediction value based on independent variables. It is mostly used for finding out the relationship between variables and forecasting. Different regression models differ based on – the kind of relationship between dependent and independent variables, they are considering and the number of independent variables being used.
```{python}

import numpy as np
x=np.array([1,2,3,4,5,6,7,8])
y=4*x+6.754
nr=np.sum((np.multiply(y-np.mean(y),x-np.mean(x))))
dnr=np.sum((x-np.mean(x))**2)
# print(nr)
# print(dnr)
theta_1=nr/dnr
theta_0=np.mean(y)-theta_1*np.mean(x)
print("slope :",theta_1)
print("Intercept :",theta_0)
```
