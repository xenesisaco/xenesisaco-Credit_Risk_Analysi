Credit_Risk_Analysi
## Overview

For this module, we built several machine learning models, using python, to predict credit risk.

- Utilizing SMOTE and RandomOverSampler algorithms, we oversampled the data. 
- Using ClusterCentroids we undersampled the data. 
- Using both under and over sampling with SMOTEENN algorth.
- With BalanceRandomForestClassifier and EasyEnsebleClassifier we compares the machine learning models to minimize bias. 

Using these methods, we will be able to classify and predict and recommend potential credit risk. 


## Results
### RandomOverSampler
Balanced accuracy score is 65%.
The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%

![1 3](https://user-images.githubusercontent.com/98041751/172724989-f3f96fd9-26a2-491d-a89f-2e6114c8ac8f.png)

![1 2](https://user-images.githubusercontent.com/98041751/172725005-b6b67a11-cfed-4f33-86a9-fd517daf24cb.png)

![1 1](https://user-images.githubusercontent.com/98041751/172725017-20918e22-58ef-40d6-865a-fa03d23d9998.png)


### SMOTE model
The results are pretty similar to the previous model.
The balanced accuracy score is 64%.
The high_risk precision is about 1% only with 63% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 66%.

![2 2](https://user-images.githubusercontent.com/98041751/172725110-cf226e29-2014-4fde-8a1b-a7107ecb86d9.png)

![2 3](https://user-images.githubusercontent.com/98041751/172725131-d5267831-3ec7-4e90-934e-678469f27c6b.png)

![2 4](https://user-images.githubusercontent.com/98041751/172725143-d19c00eb-c059-49e8-9701-601ee19e316b.png)

### ClusterCentroids model
Here the balanced accuracy score is down to about 52%.
The high_risk precision is still 1% only with 63% sensitivity which makes a F1 of 1%.
Due to the high number of false positives, the low_risk sensitivity is only 40%.

![3 1](https://user-images.githubusercontent.com/98041751/172725254-46bea055-db3c-4925-b42d-ae2bbcf2a14b.png)

![3 2](https://user-images.githubusercontent.com/98041751/172725264-1fdf0a63-9c0f-4edb-a5ba-ef74153a9b59.png)

![3 3](https://user-images.githubusercontent.com/98041751/172725280-1bf4ba38-2846-4513-88d9-78c9d49fb39d.png)



### SMOTEENN model
The balanced accuracy score is about 62%.
The high_risk precision is still 1% only with 68% sensitivity which makes a F1 of only 2%.
Due to the high number of false positives, the low_risk sensitivity is 57%.

![4 1](https://user-images.githubusercontent.com/98041751/172725386-840b321e-49b6-441c-8022-a803c3ddeecc.png)

![4 2](https://user-images.githubusercontent.com/98041751/172725393-1f3a9046-f4b3-4b25-8d1f-dbca91930bce.png)

![4 3](https://user-images.githubusercontent.com/98041751/172725525-d5d87736-04df-4695-bb80-780f459ad8df.png)


### BalancedRandomForestClassifier 
The balanced accuracy score improved to about 79%.
The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.
Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.

![5 1](https://user-images.githubusercontent.com/98041751/172725635-2482d2ed-1770-458d-a724-7b759d4c6966.png)


![5 2](https://user-images.githubusercontent.com/98041751/172725644-3f85f926-4199-4a03-a99b-a1cd48bc31ff.png)

![5 3](https://user-images.githubusercontent.com/98041751/172725655-979a6ae0-54da-4e0b-8451-9fc278f3a0b0.png)


### EasyEnsembleClassifier
Now, the balanced accuracy score is high to about 93%.
The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.
Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.

![1 1](https://user-images.githubusercontent.com/98041751/172725768-c49876b2-a026-40d8-bc32-74b3903f843c.png)

![1 2](https://user-images.githubusercontent.com/98041751/172725776-7577b076-4c73-4cdb-8c38-adaa8c38df7e.png)

![1 3](https://user-images.githubusercontent.com/98041751/172725788-4e57d346-2845-4d39-8672-8665deab4ad7.png)



## Summary

All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high.
The Ensemble models brought a lot more improvment specially on the sensitivity of the high risk credits.
The EasyEnsembleClassifier model shows a recall of 92% so it detects almost all high risk credit. On another hand, with a low precision, a lot of low risk credits are still falsely detected as high risk which would penalize the bank's credit strategy and infer on its revenue by missing those business opportunities.
For those reasons I would not recommend the bank to use any of these models to predict credit risk.


