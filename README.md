# Credit Risk Analysis:

## Review of LendingClub’s peer-to-peer lending services.

### Overview of the Project

The purpose of this project is to analyze the data from LendingClub’s peer-to-peer lending services company and predict if a loan application was high or low risk.  Credit risk data is inherently unbalanced since there are significantly more good loans than risky loans. Analyzing the data requires using several different techniques in order to evaluate it.  

For this analysis the libraries and algorithms of several different machine learning models were used to train and test the data.  Some of the methods used, includes oversampling, undersampling, and combination sampling along with boosting and bagging.  These methods allow for easier evaluation of and comparison of the results.

### Results:

There were six machine learning models used in the evaluation of the data.  The data for each was cleaned, split between training and testing sets for the evaluation.  The results of the models are:

-	Naïve Random Oversampling: had a balanced accuracy score of 64%, a 1% precision rate for high-risk, and a recall rate of 69%
	
![Naive cm](https://user-images.githubusercontent.com/99366022/174693063-98ea790b-b673-4165-8f34-484530227ade.png)

-	SMOTE Oversampling: had a balanced accuracy score of 66%, a 1% precision rate for high-risk, and a recall rate of 63%
	
![SMOTE cm](https://user-images.githubusercontent.com/99366022/174693080-f3d1d4f0-d1b9-417a-ae2f-d281d520588e.png)

-	Undersampling: had a balanced accuracy score of 55%, a 1% precision rate for high-risk, and a recall rate of 69%
	
![Undersampling cm](https://user-images.githubusercontent.com/99366022/174693848-6b164586-1939-4196-991f-b83ba24a8c86.png)

-	Combination (Over and Under) Sampling: had a balanced accuracy score of 65%, a 1% precision rate for high-risk, and a recall rate of 72%
	
![Combination cm](https://user-images.githubusercontent.com/99366022/174693092-4fdc5c3b-ef82-48c0-84ba-6ba8d637231d.png)

-	Balanced Random Forest Classifier: had a balanced accuracy score of 78%, a 4% precision rate for high-risk, and a recall rate of 64%
	
![Balanced cm](https://user-images.githubusercontent.com/99366022/174693100-99798aa3-3375-4e91-9b3c-b7d84c8739ff.png)

-	Easy Ensemble AdaBoost Classifier: had a balanced accuracy score of 93%, a 7% precision rate for high-risk, and a recall rate of 92% 
	  
![Easy cm](https://user-images.githubusercontent.com/99366022/174693106-2da3ea98-16c0-4418-a2bc-040778a748ba.png)

### Summary

If I had to pick one model to use, I would use the Easy Ensemble AdaBoost Classifier.  This model had the overall highest balanced accuracy score at 93% with an F1 score of 13%. The other models balanced accuracy score ranged between 78% and 55%.  This model had a precision rate of 7% and most of the other models had a precision rate of 1%.  The one exception was the Balanced Random Forest Classifier with a precision rate of 4%. The F1 score for five of the other models were 2% or less.  Again, the one exception was the Balanced Random Forest Classifier at 8%.

Credit risk is difficult to predict due to the significantly unbalanced dataset.  This analysis shows that even after running the data through several algorithm-based machine learning models the results were not impressive.  For these reasons, I wouldn’t recommend any of these models to identify high vs. low risk loans.
