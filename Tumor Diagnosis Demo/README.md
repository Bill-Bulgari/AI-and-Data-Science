# Tumor Diagnosis Demo

This project is a compact Machine Learning notebook for binary tumor classification using the Wisconsin breast-cancer dataset available through `scikit-learn`. The notebook demonstrates a full supervised-learning workflow: loading a labeled medical dataset, standardizing numerical predictors, visualizing representative features, training a linear large-margin classifier, selecting the regularization strength by 5-fold Cross-Validation, fitting the final model, and visualizing a two-dimensional slice of the learned decision boundary.

The classifier is a Linear Support Vector Machine style model implemented with Stochastic Gradient Descent:

```python
SGDClassifier(loss='hinge', penalty='l2')
```

## Project contents

The notebook includes:

The goal is to demonstrate a full supervised-learning workflow:

- load a labeled medical dataset
- standardize the numerical predictors
- visualize two representative features
- train a linear large-margin classifier
- select the regularization strength by k-fold Cross-Validation
- fit the final model
- visualize a $2D$ slice of the learned decision boundary

## Repository structure

```text
Tumor Diagnosis Demo/
├── README.md
└── Tumor Diagnosis Demo.ipynb
```

## Requirements

The project requires Python 3 and the following Python packages:

- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `jupyter`

The notebook imports the following libraries:

```python
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn import datasets
from sklearn import preprocessing
from sklearn import linear_model
from sklearn import model_selection as ms
```

## Installation using pip

If you already have a working installation of Python 3, you can install the required packages using pip.

```bash
pip3 install numpy
pip3 install matplotlib
pip3 install seaborn
pip3 install scikit-learn
pip3 install jupyter
```

Alternatively, you can install all required packages with one command:

```bash
pip3 install numpy matplotlib seaborn scikit-learn jupyter
```

If `pip3` does not work on your system, you can use:

```bash
python3 -m pip install numpy matplotlib seaborn scikit-learn jupyter
```

On Windows, you can also use:

```bash
py -m pip install numpy matplotlib seaborn scikit-learn jupyter
```

## Purpose

The purpose of this project is to show a clean and interpretable Machine Learning workflow for a medical binary-classification problem. It connects the practical Python implementation with the underlying mathematical ideas of feature scaling, linear classification, margin-based learning, regularization, and Cross-Validation.
