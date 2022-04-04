FRAUD DETECTION

Introduction:

This project aims to build a model that suite fraud detection, which not only identifies fraud activity (high true positive rate) but also allows non- fraud transactions to go through (low false positive rate) using basic machine learning algorithms including linear approach, clustering classifiers, support vector machine, etc.

Dataset Context:

•	This dataset and the method references has been taken from Kaggle. The dataset consists of 284,807 credit card transactions with 492 fraudulent transactions. All these transactions occurred in 2 days in 2013.

•	All the data has been dimensionally reduced using Principal component analysis (PCA) to features V1, V2, …, V28 for privacy concerns, except ‘time’, ‘class’, and ‘Amount’.

•	The Class feature here is 1 for fraud cases and 0 for non-fraud cases.

•	The dataset being highly imbalanced, as the non-fraud cases are too high compared to fraud cases (0.17% of all transactions). Area under the precision recall curve is used to measure accuracy of such high imbalanced data.

•	When working with highly imbalanced data, accuracy is not reliable performance metric because if we predict everything will be in majority class (non-Fraud class here). A credit card company would always want to reduce type -II error (missed detection) as well as Type – I error (false alarm). 

The following quality measures are used in this project.
•	Precision = TP / (TP + FP)
•	Recall = TP / (TP + FN)
•	F1 score = 2 x precision x recall / (precision + recall)
•	AUCROC – Area under receiver operating curve. This curve is used to compare performance of various algorithms under various threshold settings.
•	Over here confusion matrix is also used which shows true positives, false positives, true negatives and false negatives. And the classification report is used for precision recall of the models used.

The following are parts and methods used in the project are as follows:
1.	Data Exploration
2.	Resampling of the Imbalanced Dataset
3.	Logistic Regression
4.	Decision tree classifier
5.	Random Forest Classifier
6.	Voting classifier
7.	K- means Clustering
