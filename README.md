# Credit_Risk_Analysis

## Overview of the analysis: 
The purpose of this analysis is to use different unbalanced classification machine learning models and assess the accuracy of each model's prediction on credit risk. The differentf types of models used to predict credit risk were resampling models, the SMOTEENN algorithm, and ensemble classifiers.

## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

### RandomOversampler:
![ros.png](ros.png)

- From the results above, we can see that the RandomOverSampler model generates a balanced accuracy score of about 65%.
- The classification report shows that this model's precision score for those with high risk is 1% with a recall score of 62%, while the precision score for those with low-risk is 100% with a recall score of 68%

### SMOTE Oversampling
![smote.png](smote.png)

- From the results above, we can see that the SMOTE Overseampling model generates a balanced accuracy score of about 64%.
- The classification report shows that this model's precision score is similar to that of the RandomOversampler model, with high risk at 1% and low risk at 100%. The recall score of 63% for high risk and 66% for low risk.

### ClusterCentroids Undersampling
![clustercentroids.png](clustercentroids.png)

- From the results above, we can see that the ClusterCentroids model generates a balanced accuracy score of about 51%.
- The classification report shows that this model's precision score for those with high risk is 1% with a recall score of 61%, while the precision score for those with low-risk is 100% with a recall score of 42%.

### SMOTEEN Combination Sampling
![smoteen.png](smoteen.png)

- From the results above, we can see that the SMOTEEN model generates a balanced accuracy score of about 64%.
- The classification report shows that this model's precision score for those with high risk is 1% with a recall score of 71%, while the precision score for those with low-risk is 100% with a recall score of 56%.

### BalancedRandomForestClassifier
![balancedrfc.png](balancedrfc.png)

- From the results above, we can see that the BalancedRandomForestClassifier model generates a balanced accuracy score of about 79%.
- The classification report shows that this model's precision score for those with high risk is 4% with a recall score of 67%, while the precision score for those with low-risk is 100% with a recall score of 91%.

### EasyEnsembleClassifier
![ee.png](ee.png)

- From the results above, we can see that the RandomOverSampler model generates a balanced accuracy score of about 93%.
- The classification report shows that this model's precision score for those with high risk is 7% with a recall score of 91%, while the precision score for those with low-risk is 100% with a recall score of 94%.

## Summary: 
In summary, all models had a low precision score when determining if someone's credit risk is high, and all models had a precision score of 100% when determining if someone has a low credit risk. The model with the best accuracy score was the easy ensemble classifier, which has a score of of 93%. Additionally, the recall values for the EasyEnsembleClassifier model are also higher than the other models, which indicates a lower number of false negatives. For these reasons, I recommend using the EasyEnsembleClassifier model over the rest of the models.
