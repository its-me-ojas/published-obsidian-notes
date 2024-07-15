---
{"dg-publish":true,"permalink":"/ml-simple-linear-regression/","tags":["notes"],"created":"2024-07-06T19:49:36.973+05:30","updated":"2024-07-06T19:49:36.973+05:30"}
---

![Pasted image 20240628084028.png|400](/img/user/Attachments/Pasted%20image%2020240628084028.png)
- ## Method to choose the correct line
	- ![Pasted image 20240628084404.png|400](/img/user/Attachments/Pasted%20image%2020240628084404.png)

# Jupyter Notebook - [[Salary_Data.csv]]
# Importing the libraries
```py
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
```
# Importing the dataset
```py
dataset = pd.read_csv('Salary_Data.csv')
X= dataset.iloc[:,:-1].values
y= dataset.iloc[:,-1].values
```
# Splitting the dataset into the Training set and Test set
```py
from sklearn.model_selection import train_test_split
X_train, X_test, y_train, y_test = train_test_split(X,y,test_size=0.2, random_state=0)
```
# Training the Simple Linear Regression Model on the Training Set
```py
from sklearn.linear_model import LinearRegression
regressor = LinearRegression()
regressor.fit(X_train,y_train)
```
# Predicting the Test Set Results
```py
y_pred = regressor.predict(X_test)
```
# Visualising the Training set results
```py
plt.scatter(X_train,y_train, color='red')
plt.plot(X_train, regressor.predict(X_train),color='blue')
plt.title('Salary VS Experience ( Training Set )')
plt.xlabel('Years of Experience')
plt.ylabel('Salary')
plt.show()
```
# Visualising the Test set results
```py
plt.scatter(X_test,y_test, color='red')
plt.plot(X_train, regressor.predict(X_train),color='blue')
plt.title('Salary VS Experience ( Test Set )')
plt.xlabel('Years of Experience')
plt.ylabel('Salary')
plt.show()
```