# Credit_Risk_Analysis


## Project Overvie
The purpose of this project is to anlayize data to determine credit card risk. This is done by using different techniques and libraries to evaluate models. The model is evaluated 

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

The data in the csv file will be loading using RandomOverSample and SMOTE algorithems and ClusterCentroids for undersample. The ML models generated will be compared with the goal of reducin gbias. The BalancedForrestClassifier and EasyEnsembleClassifier components will be used to predict credit card risk.


### RandomOverSampler model
<p align="center">
  <img src="https://github.com/mabulhassan/Credit_Risk_Analysis/blob/main/oversampling.png">
</p>
The balanced accuracy score is 65.42%.<br>THe actual  high_risk precision is about 1% only with 63% sensitivity which makes a F1 of 2% only.<br>Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.
<br><br>

### SMOTE model
<p align="center">
  <img src="https://github.com/mabulhassan/Credit_Risk_Analysis/blob/main/smotemodel.png">
</p>
The balanced accuracy score is 62.8 which is lower than the previous model%.<br>The high_risk precision is about 1% only with 57% sensitivity which makes a F1 of 2% only.<br>Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.
<br><br>

### ClusterCentroids model
<p align="center">
  <img src="https://github.com/mabulhassan/Credit_Risk_Analysis/blob/main/clustercentroids.png">
</p>
Here the balanced accuracy score is down to about 52.9%.<br>The high_risk precision is still 1% only with 59% sensitivity which makes a F1 of 1%.<br>The risk sensitivity is only 44%m which indicates a high number of false postivies.
<br><br>

### SMOTEENN model
<p align="center">
  <img src="https://github.com/mabulhassan/Credit_Risk_Analysis/blob/main/smotemodel.png">
</p>
The balanced accuracy score is about 62.7%<br>The high_risk precision is still 1% only with 61% sensitivity which makes a F1 of only 1%.<br>Due to the high number of false positives, the low_risk sensitivity is 45%.
<br><br>

### BalancedRandomForestClassifier model
<p align="center">
  <img src="https://github.com/mabulhassan/Credit_Risk_Analysis/blob/main/balancedrandomforestcluster.png">
</p>
The balanced accuracy score improved to about 78.7%.<br>The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.<br>Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.
<br><br>

### EasyEnsembleClassifier model
<p align="center">
  <img src="https://github.com/mabulhassan/Credit_Risk_Analysis/blob/main/easyensembleclassifier.png">
</p>
The balanced accuracy score is high to about 92.5%.<br>The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.<br>Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.
<br><br>

## Summary
The percesion of all models used to determine credit risk have low percison.
However, the balancradomforestcluster and easy ensemble model show significantl higher percision with ensember model having over 92% percision rate. 

Financial institutions should use a model with higher percision. Thus, easy ensembler model should be used to predict low risk credit. All other models will likely result in false low risk prediction and could cause the bank or institution revenue losses.

