# Tumor Diagnosis Demo

This project is a compact Machine Learning notebook for binary tumor classification using the Wisconsin breast-cancer dataset available through `scikit-learn`.

The goal is to demonstrate a full supervised-learning workflow:

1. load a labeled medical dataset,
2. standardize the numerical predictors,
3. visualize two representative features,
4. train a linear large-margin classifier,
5. select the regularization strength by k-fold Cross-Validation,
6. fit the final model,
7. visualize a 2D slice of the learned decision boundary.

The notebook uses a Linear Support Vector Machine style classifier implemented through

```python
SGDClassifier(loss='hinge', penalty='l2')
