# Credit_Risk_Analysis
# Overview 

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I am to oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

# Results

Logistic Regression Over

![](https://github.com/trallen09/Credit_Risk_Analysis/blob/main/images/logisticregression.png)

Logistic Regression Under

![](https://github.com/trallen09/Credit_Risk_Analysis/blob/main/images/logisticregressionunder.png)

Logistic Regression combination

![](https://github.com/trallen09/Credit_Risk_Analysis/blob/main/images/ClusterCentroids.png)

Balanced Random Forest

![](https://github.com/trallen09/Credit_Risk_Analysis/blob/main/images/BalancedRandomForest.png)

SMOTE

![](https://github.com/trallen09/Credit_Risk_Analysis/blob/main/images/SMOTE.png)

SMOTEENN

![](https://github.com/trallen09/Credit_Risk_Analysis/blob/main/images/SMOTEENN.png)

Easy Ensemble

![](https://github.com/trallen09/Credit_Risk_Analysis/blob/main/images/easyensemble.png)


# Recall per Model
- Logistic Regression Over - .60
- Logistic Regression Under - .58
- Logistic Regression combination - .40
- Balanced Random Forest - .87
- SMOTE - .69
- SMOTEENN - .57
- Easy Ensemble - .94




# Summary
Using recall over precision makes the most sense in predicting credit risk. Recall will find as many members of the positive class as possible making your prediciton more conservative than having precision. I will use recall for determining the best model.

The modle using the Easy Ensemble Classifier produced the highest recall with .94. Therefore, credit risk is best determined using Easy Ensemble AdaBoost Classifier. 
