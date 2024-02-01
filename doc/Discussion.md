# Discussion

The KNN model with k = 19 neighbours  was found to have the best accuracy, which was 73% on the testing set. THis score is much better compared to the baseline model using a DummyClassifier, which had a validation score of 52%.  
The KNN model also had a better f1 score (0.72) compared to the baseline model (0.42).  
Overall, the KNN model does moderately well in classifying the patient treatment type needed using lab results (haematocrit, haemoglobin, erythrocyte, leucocyte, thrombocyte, MCH, MCHC, MCV) in addition to age and sex. However, I had hoped to achieve better accuracy to ensure that its predictions reflect the liklihood that a patient needs in-patient or out-patient care. In this case, a correct prediction would significantly impact how suitably a patient would be cared for, thus impacting their health.  

To improve the model, less features could be used to mitigate any overfitting. It would be particularly interesting to see if the model significantly improves by only including the features that appeared to correlate with the predicted treatment (age, haematocrit levels, haemoglobin levels, erythrocyte levels, and thrombocyte levels). The features that did not appear to correlate with the predicted treatment included: sex, leucocyte levels, MCH levels, MCHC levels, MCV levels.

The prediction of patient treatment type using a binary classification model can potentially have a significant impact by saving the time of hospital staff and patients that can be redirected towards patient care.

In the future, research could look into incorporating additional factors into a classification model such as type of condition, previous hospitalization, mental state, and pain level.