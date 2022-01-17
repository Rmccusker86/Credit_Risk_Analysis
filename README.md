# Credit_Risk_Analysis

# Project Overview
We were taskes with using different machine learning models to predict credit risk. After running the models, we will look at the performance of all of them and determine the best, if any to use.

# Results
The results of the various machine learning models will be show with the Balanced Accuracy Score, Confusion Matrix, and Imbalanced Classification Report

## RandomOverSampler model
![image](https://user-images.githubusercontent.com/88358771/149686501-1a8a54bc-a083-43a1-abf9-dcbcd6a4c7ba.png)

![image](https://user-images.githubusercontent.com/88358771/149686518-9fd8e548-800b-4c68-adbd-905ab0c26542.png)

![image](https://user-images.githubusercontent.com/88358771/149686529-76e98178-7c62-4918-ad56-b0e27a2d8f51.png)

With the high risk precision at 1% with a sensitivity of 62%, it makes the F1 a 2%
The balanced accuracy score is 65%

## SMOTE
![image](https://user-images.githubusercontent.com/88358771/149686623-ff2e9a1c-8682-44dd-adea-fb9f9dd4cccc.png)

![image](https://user-images.githubusercontent.com/88358771/149686638-ed09794e-5e43-4b4c-874a-4471192dd2e6.png)

![image](https://user-images.githubusercontent.com/88358771/149686659-f53539aa-6757-441b-9a94-4e2cd22a23fa.png)

This model had very similar results to the previous one. With a balanced accuracy score being one point lower at 64%

## ClusterCentroids
![image](https://user-images.githubusercontent.com/88358771/149686762-63bd83d5-a384-4563-a79d-01a54049a57e.png)

![image](https://user-images.githubusercontent.com/88358771/149686772-ff460e31-de5e-40d3-ac44-052d2c952bb0.png)

![image](https://user-images.githubusercontent.com/88358771/149686783-2f595e97-fbbf-46f5-805f-b6e9a3118136.png)

The balanced accuracy score was much worse than the previous ones at 52%
It also contained a very high number of false positives, giving it a low_risk sensitivity of 40%

## SMOTEENN
![image](https://user-images.githubusercontent.com/88358771/149686861-75267c7e-df3f-4d32-b8f7-e55f427e53fa.png)

![image](https://user-images.githubusercontent.com/88358771/149686869-8ffe311a-8754-4a71-ab81-d950c8a96d0d.png)

![image](https://user-images.githubusercontent.com/88358771/149686879-82b73faa-4925-4873-bdba-caa21209bb98.png)

This model continues with the trend of having a balanced accuracy score of only about 62%
It also had a very high number of false positives, with only a slightly higher low_risk sensitivity of 57%

## RandomForestClassifier
![image](https://user-images.githubusercontent.com/88358771/149687197-882b646d-01a6-4180-9f40-24d11724cbbb.png)

![image](https://user-images.githubusercontent.com/88358771/149687213-42a478f6-67c1-4701-84c6-13513a7fa000.png)

![image](https://user-images.githubusercontent.com/88358771/149687222-4633f208-3754-4afe-ae17-fff980d46636.png)

The balances accuracy score impoved greatly to 79%
With a very low number of false positives, the low_risk sensitivity is now 91% with 100% precision.

# EasyEnsembleClassifier
![image](https://user-images.githubusercontent.com/88358771/149687430-e2cd4f23-9ab2-4f79-92fb-d89f706660c9.png)

![image](https://user-images.githubusercontent.com/88358771/149687446-c97ef7e2-694b-4403-a26b-c313f5d48398.png)

![image](https://user-images.githubusercontent.com/88358771/149687458-e31845f8-7d0f-4159-88d1-7a8d08938f2e.png)

With this model the balances accuracy score improved to the highest level of all at about 93%
It also carries a low number of false positives, with the low_risk sensitivity at 94% with 100% precision.

# Summary
With all the data collected with the various models to perform the credit risk analysis, they all showed a very weak precision in determining if a credit risk is high. Some performed better than others, like the Ensemble model brough a high improvement on the sensitivity of the high credit risks. While the EasyEnsemble showed a 92% recall, which means it detects almost all high-risk credit. 
All of the models carried a great number of low precisions in regards to the low risk credits falsely detected as high risk. This would never give the banks the accuracy they need to properly determing credit risk. For these reason I would not recommend the bank to use any of the models to predicy credit risk.


