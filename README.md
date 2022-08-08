# Credit_Risk_Analysis
### Overview of the analysis: 
Applying machine learning to solve a real-world challenge: credit card risk is the purpose of this analysis. Since credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans,Since credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans, this analysis used `imbalanced-learn` and `scikit-learn` libraries to build and evaluate models using resampling. The dataset is from a peer-to-peer lending services company, LendingClub. Firstly, oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk

### Results: 
#### Naive Random Oversampling


#### SMOTE Oversampling

#### Undersampling

#### Combination Under-Over Sampling

#### Balanced Random Forest Classifier

#### Easy Ensemble AdaBoost Classifier


### Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
