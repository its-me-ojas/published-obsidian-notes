---
{"dg-publish":true,"permalink":"/ml-multiple-linear-regression/","tags":["notes"],"created":"2024-07-15T15:21:51.913+05:30","updated":"2024-07-15T15:21:51.913+05:30"}
---

# CART - Classification and Regression Trees
# Multiple Linear Regression
- ![Pasted image 20240628111325.png|400](/img/user/Attachments/Pasted%20image%2020240628111325.png)
## Dummy variable trap
- ![Pasted image 20240628112520.png|400](/img/user/Attachments/Pasted%20image%2020240628112520.png)
- always omit one duplicate column
## 5 methods of building a model
1. All In
	1. prior knowledge
	2. you have to use this
	3. preparing for [[ML Backward Elimination\| backward elimination]] 
	4. [[ML Forward Selection\|ML Forward Selection]]
2. [[ML Backward Elimination\| Backward Elimination]]
3. [[ML Forward Selection\|Forward Selection]]
4. [[ML Bidirectional Elimination\|Bidirectional Elimination]]
5. Score Comparison
 - 2 - 4 steps in collective is considered stepwise regression
## No need to apply feature scaling

[[50_Startups.csv]]
```py
# importing libraries  
import numpy as np  
import matplotlib.pyplot as plt  
import pandas as pd  
  
# importing the dataset  
df = pd.read_csv('50_Startups.csv')  
X = df.iloc[:, :-1].values  
y = df.iloc[:, -1].values  
  
print(X)  
print(y)  
  
# encoding categorical data  
from sklearn.compose import ColumnTransformer  
from sklearn.preprocessing import OneHotEncoder  
  
ct = ColumnTransformer(transformers=[('encoder', OneHotEncoder(), [3])], remainder='passthrough')  
X = np.array(ct.fit_transform(X))  
print(X)  
  
# splitting the dataset into the training set and test set  
from sklearn.model_selection import train_test_split  
  
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=0)  
  
# training the multiple linear regression model on the training set  
from sklearn.linear_model import LinearRegression  
  
regressor = LinearRegression()  
regressor.fit(X_train, y_train)  
  
# predicting the test set results  
y_pred = regressor.predict(X_test)  
np.set_printoptions(precision=2)  
print(np.concatenate((y_pred.reshape(len(y_pred), 1), y_test.reshape(len(y_test), 1)), 1))
```
