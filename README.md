# Coursera-IBM-Project

This project aims to get 4 machine learning models to estimate loan payment probability. 

Models used:
- K-Nearest Neighbours
- Decision Tree
- Support Vector Machine
- Logistic Regression

The code has a section "====== Answer ======" were models are made.

### K-Fold strategy and training function
There are some design decisions for this training:

- To use K-Folds cross-validation to make a better decision for the hyperparameters for each model
- To use StratifiedKFold to keep the percentage of labels in training and testing
- To use F1-Score because these problems have imbalanced datasets and F1-Score can improve the analysis of performance
- To use a function to wrap many training iterations and make an automated decision for model selection.
- The code remains with print functions for the people who want to check the process
- After detecting the best model, is used all the original dataset to train, to take advantage of all data for the future test set

# References
- https://scikit-learn.org/stable/modules/cross_validation.html
- https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.StratifiedKFold.html
- https://machinelearningmastery.com/k-fold-cross-validation/
- https://medium.com/analytics-vidhya/accuracy-vs-f1-score-6258237beca2
- https://www.coursera.org/learn/machine-learning-with-python
