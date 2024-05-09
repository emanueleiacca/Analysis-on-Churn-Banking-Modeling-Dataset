# Churn Prediction Model

This project explores building a model to predict customer churn, allowing a business to identify customers at risk of closing their accounts. The goal is to predict on a different dataset the top 10000 clients more likely to close their account

![Customer_Churn_Prediction_Models_in_Machine_Learning](https://github.com/emanueleiacca/Analysis-on-Churn-Banking-Modeling-Dataset/assets/128679981/edc858ae-0ef5-441b-a980-a4674d9cb1b7)


## Methodology

Preprocessing: Data cleaning techniques are applied to address errors. Categorical variables are encoded for model compatibility.

Sampling: Cost-sensitive sampling helps balance the class distribution, ensuring the model prioritizes identifying churned customers.

Hyperparameter Tuning: Optuna, a hyperparameter optimization library, optimizes the parameters used by the boosting algorithms, leading to a more effective model.

Boosting Algorithms: The project utilizes four boosting algorithms: LightGBM, XGBoost, CatBoost, and Ensembling Weight Optimization. Boosting algorithms combine weak learners into a stronger learner, enhancing model performance.

Metric Evaluation: Various metrics are assessed to gauge model performance. The final metric used is Rank Probabilities which maximizes the percentage of Predicted "yes" out of the total "yes". This manual metric is similar to the recall since it maximize the TP without considering the FP but focus on a given percentile.

Interpretable Machine Learning: Shapley Values are employed to understand the significance of individual variables in the model's predictions. This helps identify factors that influence churn risk.

## Results

The model achieved the best results using Rank Probabilities, effectively identifying the most at-risk customers.
Applying a logarithmic transformation to the data did not improve model performance.
Incorporating a synthetic dataset alongside the real data contributed to test the model on new unseen data to see if it can generate.
Shapley Values provided insights into the variables with the most significant impact on churn predictions.
Conclusion

This project successfully developed a model capable of accurately predicting customer churn. By leveraging interpretable machine learning techniques, the project gained valuable understanding of the factors influencing the model's decisions.

## Tools and Libraries
All the libraries used are listed in requirements.txt
