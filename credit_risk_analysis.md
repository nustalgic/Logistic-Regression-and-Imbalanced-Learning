# Module 12 - Credit Risk Report

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

* Describe the balanced accuracy scores and the precision and recall scores of all machine learning models.
---
Accuracy: the measure of the model's performance based on the differences between predicted and actual values

  [![Screen-Shot-2022-03-27-at-8-34-39-PM.png](https://i.postimg.cc/nc40WDv0/Screen-Shot-2022-03-27-at-8-34-39-PM.png)](https://postimg.cc/gn0VXrtZ)

Precision: mostly shown through the "confusion matrix" shows the comparision between the actual and predicted values based on if they were positive (1 = healthy loan) or negative (0 = high-risk loan). You have True Positives, True Negatives, Falst Positives, and False Negatives.

[![Screen-Shot-2022-03-27-at-8-34-21-PM.png](https://i.postimg.cc/3J5t9BDk/Screen-Shot-2022-03-27-at-8-34-21-PM.png)](https://postimg.cc/Jtx3zjx8)

        precision = TPs ÷ (TPs + FPs)

Recall: also shown through the "confusion matrix" it shows the number of predictions that were correct with each model.

        recall = TPs / (TPs + FNs)

---
* Machine Learning Model 1:
  * Description of Model 1 scores
  * Accuracy: 0.95204
  * Precision: 0 = 1.00, 1 = 0.85
  * Recall: 0 = 0.99 , 1 = 0.91

---

* Machine Learning Model 2:
  * Description of Model 2 scores
  * Accuracy: 0.99367
  * Precision: 0 = 1.00 , 1 = 0.84
  * Recall: 0 = 0.99 , 1 = 0.99
---

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any.
* Which one seems to perform best? How do you know it performs best?
  * The resampled performed best. It was mostly because the datasets were the same length leading to a more accurate reading. Not only did it have a 99% accuracy score the value counts were also accurate.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
  * YES! If you do not predict whether a loan is good or bad you can potentially lose out on tons of money in interest and having loans default. The last thing you want to do is put your money behind a toxic loan.
---
If you do not recommend any of the models, please justify your reasoning.

* I don't recommend the imbalanced data sampling [Model 1]. As the amounts of data is inconsistent and makes it harder to accurately predict whether it's a healthy or high-risk loan.