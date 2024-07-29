---
{"dg-publish":true,"permalink":"/ml-decision-trees-regression/","tags":["notes"],"created":"2024-07-15T14:34:09.017+05:30","updated":"2024-07-15T15:15:38.292+05:30"}
---

![Pasted image 20240715144154.png](/img/user/Attachments/Pasted%20image%2020240715144154.png)
![Pasted image 20240715144140.png](/img/user/Attachments/Pasted%20image%2020240715144140.png)


> [!NOTE] No Feature Scaling is needed

## They are not best adapted to 2d dataset with only one feature and one dependent variable

```py
# Importing the libraries  
import numpy as np  
import pandas as pd  
import matplotlib.pyplot as plt  
  
# Importing the dataset  
dataset = pd.read_csv("../Position_Salaries.csv")  
X = dataset.iloc[:, 1:-1].values  
y = dataset.iloc[:, -1].values  
  
print("X", X)  
print("y", y)  
# Training the Decision Tree Regression Model on the whole dataset  
from sklearn.tree import DecisionTreeRegressor  
  
regressor = DecisionTreeRegressor(random_state=0)  
regressor.fit(X, y)  
# Predicting a new result  
print(regressor.predict([[6.5]]))  
  
# Visualising the Decision Tree Regression Results (high resolution)  
X_grid = np.arange(min(X), max(X), 0.1)  
X_grid = X_grid.reshape((len(X_grid), 1))  
plt.scatter(X, y, color="red")  
plt.plot(X_grid,  
         regressor.predict(X_grid),  
         color='blue'  
         )  
plt.title('Truth or Bluff (Decision Tree)')  
plt.xlabel('Position Level')  
plt.ylabel('Salary')  
plt.show()
```

![Pasted image 20240715151537.png](/img/user/Attachments/Pasted%20image%2020240715151537.png)