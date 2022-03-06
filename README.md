# Credit_Risk_Analysis

### Overview 
The purpose of this analysis is to apply diffrent machine learning algorithims to assess user credit card risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I employed different techniques to train and evaluate models with unbalanced classes. Using credit card credit dataset from LendingClub, I was able to oversample the data using the ```RandomOverSampler``` and ```SMOTE``` algorithims, and undersample the data using the ```ClusterCentriods``` algorithim. Afterwards, I used a combinatorial approach of over- and undersampling using the ```SMOTEEN``` algorithim. To reduce bias, I comapred two new machine learning models; ```BalancedRandomForestClassifier``` and ```EasyEnsembleClassifier``` to predict credit risk. 

***Dependencies:***
* imbalanced-learn
* scikit-learn

### Results

The following results are for all six machine learning algorithims are listed below:

1) ```RandomOverSampler```:
  * 62% Accuracy Score
  
  ![ros](https://github.com/DrZubi/Credit_Risk_Analysis/blob/main/Resources/images/random_oversampler.PNG)
  
2) ```SMOTE```:
  * 62% Accuracy Score
  
  ![smote](https://github.com/DrZubi/Credit_Risk_Analysis/blob/main/Resources/images/SMOTE.PNG)

3) ```ClusterCentriods```:
  * 51% Accuracy Score
  
  ![cc](https://github.com/DrZubi/Credit_Risk_Analysis/blob/main/Resources/images/cluster_centriods.PNG)

4) ```SMOTEEN```:
  * 63% Accuracy Score
  
  ![smotee](https://github.com/DrZubi/Credit_Risk_Analysis/blob/main/Resources/images/combo.PNG)

5) ```BalancedRandomForestClassifier```:
  * 79% Accuracy Score
  
  ![bb](https://github.com/DrZubi/Credit_Risk_Analysis/blob/main/Resources/images/esemble.PNG)

6) ```EasyEnsembleClassifier```:
  * 93% Accuracy Score
  
  ![ee](https://github.com/DrZubi/Credit_Risk_Analysis/blob/main/Resources/images/easy_esemble.PNG)


### Summary
Out of all the ML methods, the recommended model to use is the Easy Ensemble classifier; the model provided the highest accuracy score regarding the metrics for measuring the performance of imbalanced classes. The model also has the highest balance accuracy score; correlating to the highest exactness of data analysis. The other models, such as the Random Over sampler, SMOTE, and Cluster Centriods resulted in low F1 scores, indicating a imblanace between sensitivity and accuracy yeild. 

