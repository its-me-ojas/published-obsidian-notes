---
{"dg-publish":true,"permalink":"/ml-forward-selection/","tags":["notes"],"created":"2024-09-14T14:55:16.168+05:30","updated":"2024-07-06T19:50:10.381+05:30"}
---

Steps
1. Select a significance level to enter the model (eg SL = 0.05)
2. Fit all simple regression models y ~ x select the one with the lowest P - value
3. Keep this variable and fit all possible models with one extra predictor added to the one(s) you already have
4. Consider the predictor with the lowest p-value. If P<SL, to to step 3 , otherwise go to FIN[^1]

[^1]: FIN: keep your previous model