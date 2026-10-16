---
layout: default
title: WEI ZIMING | Data Science Portfolio
---

# WEI ZIMING
## Data Science Portfolio

I am a CISC7204 student exploring how data analysis and clear visual communication can answer focused research questions. This portfolio documents an introductory, reproducible analysis and the steps I plan to improve next.

### Technical skills demonstrated in this project
Python · pandas · Matplotlib · exploratory data analysis · scikit-learn pipelines · stratified cross-validation · GitHub documentation

---

## Featured project: Reading Iris measurements

**Research question:** Do petal length and width distinguish Iris species more clearly than sepal length and width?

**Status:** Ongoing — core analysis and an explicitly simulated review improvement are complete; actual classmate feedback is pending.

### Results at a glance

| Measurements used | Mean accuracy across five folds |
|---|---:|
| Petal length and width | 95.3% |
| Sepal length and width | 81.3% |

**Difference: 14.0 percentage points in this evaluation.** Accuracy means the proportion of flowers assigned the correct species. Five-fold cross-validation divides the data into five groups: each model learns from four groups and is tested on the remaining group, repeated until every group has been tested. Both models use the same groups. These averages summarize this dataset; they are not guarantees for new flowers.

The project analyzes 150 flowers across three species. Two scatter plots compare feature pairs, followed by a logistic regression comparison using identical stratified cross-validation splits. Scaling takes place inside each training fold.

![Petal length versus width, with species identified by color and marker](petal_scatter.png)

**Main visual finding:** Setosa forms a clearly separated group in petal measurements, while versicolor and virginica overlap. Petal measurements show clearer species separation than the sepal measurements below.

![Sepal length versus width, showing greater overlap between species](sepal_scatter.png)

**Calculated comparison:** Five-fold mean classification accuracy was **95.3% using petals**, compared with **81.3% using sepals**. Both models used identical folds and training-only scaling. These are within-dataset results, not a guarantee for new samples.

**Interpretation:** The sepal plot shows why a visually plausible feature may still be less useful for distinguishing classes. The project README includes the calculated cross-validation comparison and exact reproduction instructions.

**Limitation:** This small, historical and balanced teaching dataset does not establish performance on flowers collected in a new environment. Visual separation and cross-validation accuracy do not prove causation or universal generalization.

[Explore the project code, results and README →](https://github.com/WEIZIMING369/data-science-project)

### Data and reproducibility
Data: [UCI Iris](https://archive.ics.uci.edu/dataset/53/iris), Fisher (1936), [DOI 10.24432/C56C76](https://doi.org/10.24432/C56C76), licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Measurements are in centimetres. The project includes the original source file, pinned Python dependencies and a runnable analysis script.

### Review and next improvements

An AI-generated simulated review suggested making the comparison easier to find and explaining the evaluation. I added the table and plain-language explanation above. This was not a real classmate review. [Read the transparent review log](review-log.md).

### Next improvements
Obtain classmate feedback on the purpose, finding and limitation, then implement and document one specific improvement. Future analysis could inspect misclassified flowers and evaluate an independent dataset.

---

Prepared for CISC7204 Practice 09 with assistance from OpenAI Codex. Public content contains no student ID or private contact information.


