# Random_Forest

Problem Statement:

Analyzing the Purchase details where their products are advertised in the Social media. 

Problem Description:

The Data contains detailed information about the person who using social media (like user_id, age, income, purchasing status). We here to classify the person who using social media where purchasing the product or not by using Random forest Classification. 

Code:

- #types : The data having 4 integer types and 1 object type. Totally, there are 400 observations and 5 features in the data.

- #checking for duplicates : No duplicate rows in the data.

- #checking for null values : There is no null values in the data.

- #features scaling : User_id, gender, age, salary are in different scaling. So we encode those features into same scale.

- #Gridsearchcv : Gridsearchcv is used in this model for the best fit. It shows that the decision tree with the criterion as gini, max_features as auto, n_estimators as 200 and max_depth as 4 to get the best fit with good accuracy.

-precision    recall  f1-score   support

           0       0.95      0.91      0.93        79
           1       0.84      0.90      0.87        41

    accuracy                           0.91       120
   macro avg       0.89      0.91      0.90       120
weighted avg       0.91      0.91      0.91       120

Accuracy :  0.9083333333333333
AUC score :  0.9069157147267675
Precision quantifies the number of positive class predictions that actually belong to the positive class. (0.95 belongs to the person not purchased class, 0.84 belongs to the purchased class)
Recall quantifies the number of positive class predictions made out of all positive examples in the dataset. (0.91 belongs to the person not purchased class, 0.90 belongs to the purchased class)
F-Measure provides a single score that balances both the concerns of precision and recall in one number. (0.93 belongs to the person not purchased class, 0.87 belongs to the purchased class)
It has the accuracy of 91% for the Random forest classification.
AUC (Area under ROC curve) score provides an aggregate measure of performance across all possible classification thresholds, thus it shows that this model’s prediction are 90% correct. 


Conclusion:
	We have performed Random forest classification for our data. Depending upon the social media user’s age and salary, the classification of the user purchased the product or not, which is advertised on the media. Random Forest classification was the best classifier than the decision tree, because it has the accuracy of 91% and 90% of AUC score, where decision tree has the same accuracy but with lower AUC score.




