# Fraud-Credit-Card-Kaggle
## Comprehensive Overview of Different Models:

1. *Logistic Regression (Imbalanced Data)*:
   - *Accuracy*: ~99.92%
   - *Recall*: 0.619
   - *Precision*: 0.883
   - *F1 Score*: 0.728
   - *AUC*: 0.809
   - *Details*: This model performed well in terms of accuracy but had lower recall, indicating that it missed a significant number of fraud cases.

2. *Logistic Regression with Class Weight (Balanced Data)*:
   - *Accuracy*: ~97.70%
   - *Recall*: 0.911
   - *Precision*: 0.065
   - *F1 Score*: 0.121
   - *AUC*: 0.944
   - *Details*: Adjusting for class imbalance improved recall but drastically reduced precision, which could lead to many false positives.

3. *Logistic Regression with Different Regularisation Strengths*:
   - *C=0.01*:
     - *Accuracy*: ~93.11%
     - *Recall*: 0.891
     - *Precision*: 0.100
     - *F1 Score*: 0.180
     - *AUC*: 0.939
   - *C=0.1*:
     - *Accuracy*: ~97.40%
     - *Recall*: 0.925
     - *Precision*: 0.058
     - *F1 Score*: 0.109
     - *AUC*: 0.950
   - *C=1*:
     - *Accuracy*: ~96.82%
     - *Recall*: 0.918
     - *Precision*: 0.048
     - *F1 Score*: 0.090
     - *AUC*: 0.943
   - *Details*: Lower values of C provided better recall but at the cost of precision. The higher the value of C, the model leaned towards better accuracy and AUC, but precision remained low across the board.

4. *Decision Tree*:
   - *Accuracy*: ~99.93%
   - *Recall*: 0.762
   - *Precision*: 0.836
   - *F1 Score*: 0.797
   - *AUC*: 0.881
   - *Details*: The Decision Tree performed very well in terms of accuracy and precision, but it did not capture as many fraud cases as other models, resulting in a lower recall.

5. *Naive Bayes*:
   - *Accuracy*: ~97.85%
   - *Recall*: 0.837
   - *Precision*: 0.063
   - *F1 Score*: 0.118
   - *AUC*: 0.908
   - *Details*: The Naive Bayes model had high accuracy but struggled with precision and recall, leading to a model that might not be the best choice for fraud detection.

### Conclusion:
Among the models, *Decision Tree* and *Logistic Regression with class weights* offer a good balance between precision and recall, depending on whether higher accuracy or higher recall is the priority. However, the *Random Forest* (not detailed here but generally robust in feature selection and prediction) could be considered as the recommended choice if it was included, due to its ability to handle imbalanced datasets effectively and provide a more comprehensive evaluation across all metrics.
