---
layout: default
title: Review and improvement log
---

# Review and improvement log

**Purpose**: Using the UCI Iris dataset (150 flowers, three species) to answer one focused question — do petal length and width distinguish Iris species more clearly than sepal length and width? — while demonstrating a reproducible workflow, from exploratory visualisation to comparing logistic regression models on both feature sets under identical stratified cross-validation splits, with scaling confined to each training fold to prevent leakage.

**Main findings**: In the petal plot setosa is clearly separated while versicolor and virginica overlap; the sepal plot shows substantial class mixing. Mean five-fold accuracy was **95.3%** with petals versus **81.3%** with sepals — a **14.0-point** gap on identical folds — showing that a visually plausible feature need not be useful, and that these within-dataset results do not guarantee performance on new samples.

**One limitation**: The dataset is small, historical and perfectly balanced, so it cannot support the claim that the model still works on flowers from a new environment; moreover, the current review is an AI simulation, leaving real classmate feedback missing.

**Improvement suggestion**: Add a compact accuracy table before the charts — petals 95.3%, sepals 81.3%, a 14.0-point gap — so readers grasp the conclusion at a glance and the charts can explain why. Also explain five-fold cross-validation in plain language: split the data into five groups, train on four and test on the remaining one, repeat until every group has been tested, then average the results; both models must use identical groups to keep the comparison fair. That way readers without a machine learning background see where 95.3% comes from and know it applies only to this dataset.
