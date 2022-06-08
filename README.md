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
Sensitivity is about 62% while precision in high_risk is about 1%. This makes a F1 of 2% only.
Precision is almost 100% due to the large number of the low_risk population, with a sensitivity of 68%.

![1 3](https://user-images.githubusercontent.com/98041751/172724989-f3f96fd9-26a2-491d-a89f-2e6114c8ac8f.png)

![1 2](https://user-images.githubusercontent.com/98041751/172725005-b6b67a11-cfed-4f33-86a9-fd517daf24cb.png)

![1 1](https://user-images.githubusercontent.com/98041751/172725017-20918e22-58ef-40d6-865a-fa03d23d9998.png)


### SMOTE model
This model resembles the previous model. 
The balanced accuracy score is 64%.
Sensitivity is only 63% with a high_risk precision of about 1%. This makes F1 of 2% only.
Precision is almost 100% due to the large number of the low_risk population, with a sensitivity of 66%.

![2 2](https://user-images.githubusercontent.com/98041751/172725110-cf226e29-2014-4fde-8a1b-a7107ecb86d9.png)

![2 3](https://user-images.githubusercontent.com/98041751/172725131-d5267831-3ec7-4e90-934e-678469f27c6b.png)

![2 4](https://user-images.githubusercontent.com/98041751/172725143-d19c00eb-c059-49e8-9701-601ee19e316b.png)

### ClusterCentroids model
Balance accuracy is about 52%.
Senesitivity only is 63% with a high_risk precision is still 1%. This makes F1 of 1%.
Low_risk is only 40% due to the high number of false positives.

![3 1](https://user-images.githubusercontent.com/98041751/172725254-46bea055-db3c-4925-b42d-ae2bbcf2a14b.png)

![3 2](https://user-images.githubusercontent.com/98041751/172725264-1fdf0a63-9c0f-4edb-a5ba-ef74153a9b59.png)

![3 3](https://user-images.githubusercontent.com/98041751/172725280-1bf4ba38-2846-4513-88d9-78c9d49fb39d.png)



### SMOTEENN model
The balanced accuracy score is about 62%.
Sensitivity is only 68% with a high_risk precision at 1%. This makes F1 of only 2%.
Due to the high number of false positives, the low_risk sensitivity is 57%.

![4 1](https://user-images.githubusercontent.com/98041751/172725386-840b321e-49b6-441c-8022-a803c3ddeecc.png)

![4 2](https://user-images.githubusercontent.com/98041751/172725393-1f3a9046-f4b3-4b25-8d1f-dbca91930bce.png)

![4 3](https://user-images.githubusercontent.com/98041751/172725525-d5d87736-04df-4695-bb80-780f459ad8df.png)


### BalancedRandomForestClassifier 
The balanced accuracy score improved to about 79%.
Sensitivity is only 67% with a high_risk precision at a low 4%, making the F1 of only 7%.
The low_risk sensitivity is at 91% due to a lower number of false positives, with 100% presicion.

![5 1](https://user-images.githubusercontent.com/98041751/172725635-2482d2ed-1770-458d-a724-7b759d4c6966.png)


![5 2](https://user-images.githubusercontent.com/98041751/172725644-3f85f926-4199-4a03-a99b-a1cd48bc31ff.png)

![5 3](https://user-images.githubusercontent.com/98041751/172725655-979a6ae0-54da-4e0b-8451-9fc278f3a0b0.png)


### EasyEnsembleClassifier
The balanced accuracy score is high at around 93%.
WIth only 91% sensitivity and with the high_risk precision is still low at 7%. makes a F1 of only 14%.
With low_risk sensitivity at 94% due to a lower number of false positives, with 100% presicion.

![1 1](https://user-images.githubusercontent.com/98041751/172725768-c49876b2-a026-40d8-bc32-74b3903f843c.png)

![1 2](https://user-images.githubusercontent.com/98041751/172725776-7577b076-4c73-4cdb-8c38-adaa8c38df7e.png)

![1 3](https://user-images.githubusercontent.com/98041751/172725788-4e57d346-2845-4d39-8672-8665deab4ad7.png)



## Summary
The risk is high since all models used show weak precision. 
However, high improvement on the sensitivity of high risk credits can be seen through the Ensemble model. 
With a recall of 92%, EasyEnsembleClassifier model detects all high risk credi while, with a low precision, the bank's credit strategy is penatalized because this method detects low_risk credit falsely as high_risk, which can mendle with its profit. For this reason, the bank should not use any of these models to predict credit risk. 
