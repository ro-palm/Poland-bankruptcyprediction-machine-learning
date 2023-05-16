# Report

# **MLG-2-Assignment1-Group-6**
## -- Team Members --
* ### Vuyo Fortune Mathe : 578376
* ### Roan Palm : 578632
* ### Henko Meyer : 578420

##Abstract
This report presents a classification model for bankruptcy prediction in companies operating in Poland. The model was built using a GradientBoostingClassifier algorithm, and its performance was evaluated on a dataset containing 66 features and a binary label indicating bankruptcy (True/False). The dataset was split into training and testing sets, and the target vector was resampled using a RandomOverSampler to address the class imbalance. Hyperparameters were tuned using GridSearchCV, and the model achieved an accuracy of 0.892, precision of 0.899, recall of 0.0892, and F1-score of 0.892 on the testing set. Feature importance analysis revealed the top 10 most important features for bankruptcy prediction. The developed model has practical importance for businesses, investors, and financial institutions, and can contribute to the stability and growth of the economy.

## Introduction
This report presents the results of a classification task on bankruptcy prediction for companies in Poland. The dataset used for this task contains 64 features and a binary label indicating bankruptcy (True/False). The objective of this task is to build a model that can accurately predict whether a company will go bankrupt or not.
The bankruptcy prediction model presented in this report has significant practical importance for businesses, investors, and financial institutions operating in Poland. By accurately predicting the likelihood of a company going bankrupt, the model can help businesses and investors make informed decisions about investment, financing, and risk management. Financial institutions can also use the model to identify high-risk borrowers and take appropriate measures to mitigate the risk of loan defaults.

Furthermore, this model can have broader economic implications. Bankruptcy can have a significant impact on the economy, causing job losses, supply chain disruptions, and a decline in economic activity. Early detection of companies at risk of bankruptcy can help prevent such negative consequences and allow for timely interventions to support struggling businesses. Overall, the development of accurate bankruptcy prediction models can contribute to the stability and growth of the economy.
Back to this assignment, we used the GradientBoostingClassifier algorithm to predict whether a company will go bankrupt or not based on 66 features. We performed the following steps:

1.	Loaded the data and prepared it for modeling by dropping any features with missing values.
2.	Split the data into training and testing sets, with 80% of the data for training and 20% for testing.
3.	Resampled the target variable using the Random Over Sampling technique to address class imbalance.
4.	Trained a GradientBoostingClassifier model on the training set using cross-validation and GridSearchCV to tune hyperparameters.
5.	Evaluated the model on the testing set and reported the accuracy, precision, recall, and F1-score.
6.	Computed the feature importance of the model and reported the top 10 most important features.
We used the Random Over Sampling technique to address the class imbalance. This technique duplicates examples from the minority class until it is balanced with the majority class. We chose this technique because it is a simple and effective way to address class imbalance. 
The other reasons why we chose Random Over Sampling
•	Improve Model Performance: Models trained on imbalanced datasets tend to be biased towards the majority class and can therefore perform poorly on the minority class. Random oversampling can help to improve the model's performance on the minority class.
•	Simple and Easy to Use: Random oversampling is a straightforward and easy-to-implement method for dealing with class imbalance.
•	Good for Small Datasets: When the dataset is small, creating duplicate samples from the minority.
.
We tuned the hyperparameters of the GradientBoostingClassifier model using GridSearchCV with a parameter grid consisting of the learning rate, number of estimators, and maximum depth. We used cross-validation with a value of 5 to evaluate the performance of the model for each set of hyperparameters. The best hyperparameters were max_depth of  10, min_samples_split of 2, n_estimators of 50.

The model achieved an accuracy of 0.892, precision of 0.899, recall of 0.892, and F1-score of 0.892 on the testing set. The confusion matrix shows that the model.
