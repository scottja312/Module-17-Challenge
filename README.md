# Module-17-Challenge
### Initial Analysis:
* This challenge assignment in supervised learning was used to classify whether a lending company could use an algorithm to identify low-risk lenders (i.e. lenders with good credits) to be approved for loans.

* In the cleaned dataset, there were 347 high-risk loans identified and 68,470 low-risk loans available to be analyzed. Overall, the dataset contained a very small percentage of high-risk loans to be identified (less than 0.5% of the total 68,817 loan data processed), leading the initial proficiency of algorithms run to be expected to identify more loans as low-risk since this data was in the majority.


* The following algorithms of RandomOverSampler, SMOTE, Undersampling (Cluster Centroids Algorithm), and Combination (SMOTEEN Algorithm) were used to determine the optimal algorithm for correctly identifying a loan as low risk.  

### Algorithm Comparison: 
Describe the precision and recall scores, as well as the balanced accuracy score for each algorithm.

#### Naive Random Oversampling:
Balanced Accuracy Score: 63.4%

##### High risk loans (Bad Credit):
* Precision score: 0.01

* Recall score: 0.74

* F1 score: 0.02


##### Low risk loans (Good Credit)
* Precision score: 1.00

* Recall score: 0.53

* F1 score: 0.69

#### SMOTE Oversampling:
Balanced Accuracy Score: 65.8%

##### High risk loans (Bad Credit):
* Precision score: 0.01

* Recall (Sensitivity) score: 0.63

* F1 score: 0.02


##### Low risk loans (Good Credit)
* Precision score: 1.00

* Recall (Sensitivity) score: 0.68

* F1 score: 0.81

#### Undersampling (Cluster Centroids Algorithm):
Balanced Accuracy Score: 54.7%

##### High risk loans (Bad Credit):
* Precision score: 0.01

* Recall (Sensitivity) score: 0.68

* F1 score: 0.01


##### Low risk loans (Good Credit)
* Precision score: 1.00

* Recall (Sensitivity) score: 0.41

* F1 score: 0.58

#### Combination (SMOTEEN Algorithm):
Balanced Accuracy Score: 64.4%

##### High risk loans (Bad Credit):
* Precision score: 0.01

* Recall (Sensitivity) score: 0.72

* F1 score: 0.02


##### Low risk loans (Good Credit)
* Precision score: 1.00

* Recall (Sensitivity) score: 0.57

* F1 score: 0.72


### Analysis of model performance and final recommendation:
Ultimately for a loan lending company, it is ideal to have an algorithm that can identify high risk lenders (bad credit), and maximize the amount of low-risk lenders (good credit) to continously keep the loan company in business. Using this imbalanced dataset, the accuracy score could have been higher across all four algorithms, but this was overall not bad since the majority of the loans were in good standing. In terms of predicting low risk lenders, the ideal algorithm would be SMOTE overampling with a balanced accuracy score of 65.8%, and an F1 score of 81 (highest of all low risk loans tried for all four algorithms). In terms of predicting high risk (bad credit) loans, the best algorithm is Naive random oversampling with a recall score of 74, the highest of all four algorithms. In comparison of oversampling versus undersampling techniques, oversampling would be the ideal algorithm for identifying ideal low-risk lenders for clients even with the potential of misclassifying high-risk lenders among these clients.
