# Credit_Risk_Analysis
### Overview of the analysis: 
Applying machine learning to solve a real-world challenge: credit card risk is the purpose of this analysis. Since credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans,Since credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans, this analysis used `imbalanced-learn` and `scikit-learn` libraries to build and evaluate models using resampling. The dataset is from a peer-to-peer lending services company, LendingClub. Firstly, oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk

### Results: 
#### Naive Random Oversampling

![image](https://user-images.githubusercontent.com/103073631/183362801-5d88c43d-6ec7-44be-9696-2d7e0e14b620.png)

- Balanced Accuracy: 0.6249984891886339
- Precision: The precision is 0.01 for High-risk loans and 1.00 for Low-risk loans.
- Recall: High&Low risk = 0.60 ; 0.65
- F1 scores for High and Low risk: 0.02 ; 0.79

#### SMOTE Oversampling

![image](https://user-images.githubusercontent.com/103073631/183365147-963fa779-7e98-48a2-b820-a76eb3e8f1f8.png)

- Balanced Accuracy: 0.6512584051472337
- Precision: The precision is 0.01 for High-risk loans and 1.00 for Low-risk loans.
- Recall: High&Low risk = 0.64 ; 0.66
- F1 scores for High and Low risk: 0.02 ; 0.79

#### Undersampling

#### Combination Under-Over Sampling

#### Balanced Random Forest Classifier

#### Easy Ensemble AdaBoost Classifier


### Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
