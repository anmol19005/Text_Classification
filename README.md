# Text_Classification
Text classification pn Yelp data, using Multinimial Naive Bayes

Training Accuracy: 0.9485714285714286
    precision    recall  f1-score   support

           0       0.96      0.94      0.95       358
           1       0.94      0.96      0.95       342

    accuracy                           0.95       700
   macro avg       0.95      0.95      0.95       700
weighted avg       0.95      0.95      0.95       700



Validation Accuracy:0.7833333333333333
         precision    recall  f1-score   support

           0       0.79      0.78      0.78       150
           1       0.78      0.79      0.78       150

    accuracy                           0.78       300
   macro avg       0.78      0.78      0.78       300
weighted avg       0.78      0.78      0.78       300


Train-Test split - 70/30

Number of mislabeled points out of a total 300 points : 65

Misclassified :class([0, 1]), points([33, 32])
 
Correctly Classified :class([0, 1]), points([117, 118]))
 

Inferences:

Most of the correct classified points are of length 3 as well as misclassified points are also of length 3.
Naive bayes predict the tag of a text. They calculate the probability of each tag for a given text and then output the tag with the highest one. For some uncommon words it is performing well for example ‘mortize’, just for a single word it is classifying correctly.
Length greater than 8 highly misclassified, probability with larger length gets decreased, leading to misclassification.

