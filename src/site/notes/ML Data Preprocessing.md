---
{"dg-publish":true,"permalink":"/ml-data-preprocessing/","tags":["notes"],"created":"2024-07-12T08:17:07.197+05:30","updated":"2024-07-06T19:47:55.489+05:30"}
---

[[Data.csv]]
# Importing the libraries
```py
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
```
# Importing the dataset
```py
dataset = pd.read_csv('Data.csv')
X = dataset.iloc[:, :-1].values # features
y = dataset.iloc[:, -1].values # target
```
# Taking care of missing data
```py
from sklearn.impute import SimpleImputer
imputer = SimpleImputer(missing_values=np.nan,strategy='mean')
imputer.fit(X[ : ,1:3])
X[ : ,1:3] = imputer.transform(X[ : ,1:3])
```
# Encoding the categorical data
- ## Encoding the Independent variable
```py
from sklearn.compose import ColumnTransformer
from sklearn.preprocessing import OneHotEncoder
ct = ColumnTransformer(transformers=[('encoder',OneHotEncoder(),[0])],remainder='passthrough')
X=np.array(ct.fit_transform(X))
```
- ## Encoding the dependent variable
```py
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
y=le.fit_transform(y)
```
# Splitting the dataset into the Training set and Test set
```py
from sklearn.model_selection import train_test_split
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 0.2, random_state = 1)
```
# Feature Scaling
```py
from sklearn.preprocessing import StandardScaler
sc = StandardScaler()
X_train[ : , 3: ]= sc.fit_transform(X_train[ : , 3:] )
X_test[ :, 3 : ]= sc.fit_transform(X_test[ : , 3:] )
```
