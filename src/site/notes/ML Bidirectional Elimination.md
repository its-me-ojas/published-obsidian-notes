---
{"dg-publish":true,"permalink":"/ml-bidirectional-elimination/","tags":["notes"],"created":"2024-06-28T11:53:55.197+05:30","updated":"2024-07-06T19:52:37.477+05:30"}
---

Steps
1. Select a significance level to enter and to stay in the model
   eg. SLENTER=0.05 and SLSTAY=0.05
2. Perform the next step of [[ML Forward Selection\|ML Forward Selection]] ( new variables must have P<SLENTER to enter)
3. Perform all the steps of [[ML Backward Elimination\|ML Backward Elimination]] (old variables must have P< SLSTAY to stay)
4. No new variables can enter and no old variables can exit
