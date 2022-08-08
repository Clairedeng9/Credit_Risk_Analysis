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

![image](https://user-images.githubusercontent.com/103073631/183366077-2af70e0e-e1cd-4354-8039-f48b2c3e3dd3.png)

- Balanced Accuracy: 0.5107398543980726
- Precision: The precision is 0.01 for High-risk loans and 1.00 for Low-risk loans.
- Recall: High&Low risk = 0.59 ; 0.44
- F1 scores for High and Low risk: 0.01 ; 0.61

#### Combination Under-Over Sampling

![image](https://user-images.githubusercontent.com/103073631/183366304-cf2f8416-0fde-4036-9788-8f5c177ac8b6.png)

- Balanced Accuracy: 0.6163546337591808
- Precision: The precision is 0.01 for High-risk loans and 1.00 for Low-risk loans.
- Recall: High&Low risk = 0.69 ; 0.54
- F1 scores for High and Low risk: 0.02 ; 0.70

#### Balanced Random Forest Classifier

![image](https://user-images.githubusercontent.com/103073631/183366715-d49d1669-6dd0-4de7-83fc-2fcd9fe0411f.png)

- Balanced Accuracy: 0.7877672625306695
- Precision: The precision is 0.04 for High-risk loans and 1.00 for Low-risk loans.
- Recall: High&Low risk = 0.67 ; 0.91
- F1 scores for High and Low risk: 0.07 ; 0.95

#### Easy Ensemble AdaBoost Classifier

![image](https://user-images.githubusercontent.com/103073631/183366894-3283abd5-28a0-458e-ac7c-9d323f8a31a3.png)

- Balanced Accuracy: 0.925427358175101
- Precision: The precision is 0.07 for High-risk loans and 1.00 for Low-risk loans.
- Recall: High&Low risk = 0.91 ; 0.94
- F1 scores for High and Low risk: 0.14 ; 0.97

### Summary: 
Precision is the measure of how reliable a positive classification is and a low precision is indicative of a large number of false positives; Recall is the ability of the classifier to find all the positive samples and a low recall is indicative of a large number of false negatives; F1 score is a weighted average of the true positive rate (recall) and precision, where the best score is 1.0 and the worst is 0; Support is the number of actual occurrences of the class in the specified dataset. From above different models, the highest model's accuracy is `****0.925427358175101****`, which belongs to Easy Ensemble AdaBoost Classifier, and the precision and recall are good enough to state that the model will be good at classifying credit risk loans. Therefore, I will recommendation on the ****Easy Ensemble AdaBoost Classifier**** model to use.
