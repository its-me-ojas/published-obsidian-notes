---
{"dg-publish":true,"permalink":"/ml-logistic-regression/","tags":["notes"],"created":"2024-09-14T14:55:04.104+05:30","updated":"2024-07-29T07:00:35.163+05:30"}
---


#### predicting a categorical dependent variable from a number of independent variables
![Pasted image 20240716081432.png](/img/user/Attachments/Pasted%20image%2020240716081432.png)
#### Increasing the number of dependent variables
![Pasted image 20240716081533.png](/img/user/Attachments/Pasted%20image%2020240716081533.png)

### Maximum Likelihood
![Pasted image 20240716081853.png](/img/user/Attachments/Pasted%20image%2020240716081853.png)
Take multiple graphs and just compare the maximum likelihood
![Pasted image 20240716081951.png](/img/user/Attachments/Pasted%20image%2020240716081951.png)

# Code using

![[breast_cancer.csv]]

```py
import pandas as pd

dataset = pd.read_csv('../breast_cancer.csv')  
X = dataset.iloc[:, 1:-1].values  
y = dataset.iloc[:, -1].values

from sklearn.model_selection import train_test_split  
  
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=0)

from sklearn.linear_model import LogisticRegression  
  
classifier = LogisticRegression(random_state=0)  
classifier.fit(X_train, y_train)

y_pred = classifier.predict(X_test)

from sklearn.metrics import confusion_matrix  
  
cm = confusion_matrix(y_test, y_pred)  
print(cm)

from sklearn.model_selection import cross_val_score  
  
accuracies = cross_val_score(estimator=classifier, X=X_train, y=y_train, cv=10)  
print("Accuracy: {:.2f} %".format(accuracies.mean() * 100))  
print("Standard Deviation: {:.2f} %".format(accuracies.std() * 100))
```