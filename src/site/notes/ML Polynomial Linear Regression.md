---
{"dg-publish":true,"permalink":"/ml-polynomial-linear-regression/","tags":["notes"],"created":"2024-07-06T19:49:52.758+05:30","updated":"2024-07-06T19:49:52.758+05:30"}
---

[[Position_Salaries.csv]]

```py
# importing libraries  
import numpy as np  
import matplotlib.pyplot as plt  
import pandas as pd  
  
# importing the dataset  
df = pd.read_csv('Position_Salaries.csv')  
X = df.iloc[:, 1:-1].values  
y = df.iloc[:, -1].values  
  
print(X)  
print(y)  
  
# Training the polynomial linear regression model on the training  
from sklearn.linear_model import LinearRegression  
  
lin_reg = LinearRegression()  
lin_reg.fit(X, y)  
  
# Training the polynomial regression model on the whole dataset  
from sklearn.preprocessing import PolynomialFeatures  
  
poly_reg = PolynomialFeatures(degree=4)  
X_poly = poly_reg.fit_transform(X)  
lin_req_2 = LinearRegression()  
lin_req_2.fit(X_poly, y)  
  
# Visualising the linear regression results  
plt.scatter(X, y, color='red')  
plt.plot(X, lin_reg.predict(X), color='blue')  
plt.title('Truth or Bluff (Linear Regression)')  
plt.xlabel('Position Level')  
plt.ylabel('Salary')  
plt.show()  
  
# Visualising the polynomial regression results  
plt.scatter(X, y, color='red')  
plt.plot(X, lin_req_2.predict(X_poly), color='blue')  
plt.title('Truth or Bluff (Polynomial Regression)')  
plt.xlabel('Position Level')  
plt.ylabel('Salary')  
plt.show()  
  
# Visualising the polynomial regression results (for higher resolution and smoother curve)  
X_grid = np.arange(min(X), max(X), 0.1)  
X_grid = X_grid.reshape((len(X_grid), 1))  
plt.scatter(X, y, color='red')  
plt.plot(X_grid, lin_req_2.predict(poly_reg.fit_transform(X_grid)), color='blue')  
plt.title('Truth or Bluff (Polynomial Regression)')  
plt.xlabel('Position Level')  
plt.ylabel('Salary')  
plt.show()  
  
# Predicting a new result with linear regression  
print(lin_reg.predict([[6.5]]))  
  
# Predicting a new result with polynomial regression  
print(lin_req_2.predict(poly_reg.fit_transform([[6.5]])))
```

![Pasted image 20240628184424.png|300](/img/user/Attachments/Pasted%20image%2020240628184424.png) ![Pasted image 20240628184445.png|300](/img/user/Attachments/Pasted%20image%2020240628184445.png)
![Pasted image 20240628184454.png|300](/img/user/Attachments/Pasted%20image%2020240628184454.png) ![Pasted image 20240628184501.png|300](/img/user/Attachments/Pasted%20image%2020240628184501.png)