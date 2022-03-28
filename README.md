# Imbalanced-Learn & Logistic Regression

Module 12 Challenge

[![Screen-Shot-2022-03-27-at-8-39-09-PM.png](https://i.postimg.cc/tRmF50Bq/Screen-Shot-2022-03-27-at-8-39-09-PM.png)](https://postimg.cc/G9GBLf0V)

# Background

Credit risk poses a classification problem that’s inherently imbalanced. This is because healthy loans easily outnumber risky loans. In this Challenge, I’ll use various techniques to train and evaluate models with imbalanced classes. I’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

---

## Technologies

The data we're analyzing comes from a jupyter notebook that we'll create and import files to. We'll be using Python to run and read our data. 

* [jupyter] - (https://github.com/jupyter/notebook) - Helps us run our code and get the information we need from the data listed in csv files.

---

## Installation Guide

In order for us to get the data we need we must import pandas, plots and the csv files we want to observe.

```python
# Import the modules
import numpy as np
import pandas as pd
from pathlib import Path
from sklearn.metrics import balanced_accuracy_score
from sklearn.metrics import confusion_matrix
from imblearn.metrics import classification_report_imbalanced
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.preprocessing import StandardScaler
from imblearn.over_sampling import RandomOverSampler

import warnings
warnings.filterwarnings('ignore')
```


## Usage
---
## Evaluating the model’s performance by doing the following:

* Calculate the accuracy score of the model.

* Generate a confusion matrix.

* Print the classification report.

```python
# Print the balanced_accuracy score of the model 
accuracy = balanced_accuracy_score(y_test, y_pred_test2)
print(accuracy)
```
[![Screen-Shot-2022-03-27-at-8-34-39-PM.png](https://i.postimg.cc/nc40WDv0/Screen-Shot-2022-03-27-at-8-34-39-PM.png)](https://postimg.cc/gn0VXrtZ)

---
```python
# Generate a confusion matrix for the model
training_matrix2 = confusion_matrix(y_test, y_pred_test2)
training_matrix2
```
[![Screen-Shot-2022-03-27-at-8-34-21-PM.png](https://i.postimg.cc/3J5t9BDk/Screen-Shot-2022-03-27-at-8-34-21-PM.png)](https://postimg.cc/Jtx3zjx8)

---
```python
# Print the classification report for the model
training_report2 = classification_report_imbalanced(y_test, y_pred_test2)
print(training_report2)
```
[![Screen-Shot-2022-03-27-at-8-34-08-PM.png](https://i.postimg.cc/Hxr6vv2y/Screen-Shot-2022-03-27-at-8-34-08-PM.png)](https://postimg.cc/vgd7czCY)

---
## Contributors

Brought to you by Elgin Braggs Jr.

---

## License

MIT