---
{"dg-publish":true,"permalink":"/ml-backward-elimination/","tags":["notes"],"created":"2024-09-14T14:53:22.523+05:30","updated":"2024-07-06T19:50:05.853+05:30"}
---

Steps
1. select a significance level to stay in the model (eg SL = 0.05)
2. Fit the full model with all possible predictors
3. Consider the predictor with the highest P value. If P > SL, go to step 4, otherwise go to FIN[^1]
4. Remove the predictor
5. Fit the model without this variable
6. rebuild the model

[^1]: FIN: your model is ready