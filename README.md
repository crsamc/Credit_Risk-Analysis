# Credit_Risk_Analysis
## Overview
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once done, evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.
## Results
- Naive Random Oversampling

![Screenshot (4)](https://user-images.githubusercontent.com/101649525/193466851-a5b36ad2-ec80-4c7b-a5d6-be10a6f371fc.png)

1. Balanced Accuracy: 0.6377849893840322
2. Precision: The precision is low (0.01) for High-risk loans and is high (1.00) for Low-risk loans.
3. Recall: High/Low risk = .61/.67

- SMOTE Oversampling 

![Screenshot (5)](https://user-images.githubusercontent.com/101649525/193466856-0ec3db7f-9832-4dfc-861c-813866fdd230.png)

1. Balanced Accuracy: 0.642772681307436
2. Precision: The precision is low (0.01) for High-risk loans and is high (1.00) for Low-risk loans.
3. Recall: High/Low risk = .62/.66

- Undersampling

![Screenshot (6)](https://user-images.githubusercontent.com/101649525/193466867-3c748dc8-130e-4928-9e52-106deb28ccba.png)

1. Balanced Accuracy: 0.5221827396851872
2. Precision: The precision is low (0.01) for High-risk loans and is high (1.00) for Low-risk loans.
3. Recall: High/Low risk = .60/.45

- Combination Under-Over Sampling

![Screenshot (7)](https://user-images.githubusercontent.com/101649525/193466873-591bc008-99fc-4dd5-aeb0-778f99998963.png)

1. Balanced Accuracy: 0.6087159714919967
2. Precision: The precision is low (0.01) for High-risk loans and is high (1.00) for Low-risk loans.
3. Recall: High/Low risk = .67/.55

- Balanced Random Forest Classifier

![Screenshot (8)](https://user-images.githubusercontent.com/101649525/193466876-a98a9318-9261-4db3-b924-e4995e2c000d.png)

1. Balanced Accuracy: 0.795829959187949
2. Precision: Precision: The precision is low (0.03) for High-risk loans and is high (1.00) for Low-risk loans.
3. Recall: High/Low risk = .71/.88

- Easy Ensemble AdaBoost Classifier

![Screenshot (9)](https://user-images.githubusercontent.com/101649525/193466881-42b8e721-6dea-4c61-8ff7-b5c146f474a2.png)

1. Balanced Accuracy: 0.9263912558266958
2. Precision: Precision: The precision is low (0.08) for High-risk loans and is high (1.00) for Low-risk loans.
3. Recall: High/Low risk = .91/.94

## Summary
For the credit card data set, the Easy Ensemble AdaBoost Classifier is the best model with its .93 balanced accuracy. The other models ranged from .52 to .80 balanced accuracy. The precision for all models were similar. The recall score also needs to fall within 0 and 1, with numbers closer to 1 being the better model. The Easy Ensemble AdaBoost Classifier had the highest recall score and would be the best choice over all of the other options.
