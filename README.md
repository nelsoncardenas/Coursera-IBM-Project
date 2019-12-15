# Coursera-IBM-Project

This project aims to get 4 machine learning models to estimate loan payment probability. 

Models used:
- K-Nearest Neghbours
- Decision Tree
- Support Vector Machine
- Logistic Regression
The code has a section "====== Answer ======" were the models are made.

### K-Fold strategie and training function
There are some desing decisions for this training:

- To use K-Folds cross-validation to make a better decision for the hiper-parameters of each model
- To use StratifiedKFold to keep percentage of labels in training and testing
- To use F1-Score because this problems have imbalanced datasets and F1-Score can improve the analysis of performance
- To use a function to wrap many trainings and make an automated decision for model selection.
- The code remains with print functions for the people who want to check the process
- After detecting the best model, is used all the original dataset to train, to take advantage of all data for the future test set

# References
https://scikit-learn.org/stable/modules/cross_validation.html
https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.StratifiedKFold.html
https://machinelearningmastery.com/k-fold-cross-validation/
https://medium.com/analytics-vidhya/accuracy-vs-f1-score-6258237beca2
