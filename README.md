# Tuning-Regularization-in-Logistic-Regression-From-Overfitting-to-Simplicity

This repository contains the code and report for a tutorial exploring how L2‑regularised logistic regression behaves on a simple two‑dimensional synthetic dataset generated with `sklearn.datasets.make_classification`. The project shows how changing the regularization strength `C` in scikit‑learn’s `LogisticRegression` affects accuracy, decision boundaries, and coefficient magnitudes.


## What this tutorial covers

- Brief theory of logistic regression and L2 regularization, including how the hyperparameter `C` controls the strength of the penalty.  
- Generation of a balanced 2D toy dataset with `make_classification` to focus on model behaviour rather than data cleaning. 
- Experiments sweeping `C` over several orders of magnitude and plotting train/validation/test accuracy to illustrate the bias–variance trade‑off.  
- Visual decision boundaries for strong, moderate, and weak regularization, plus plots of coefficient magnitudes versus `C`.  
- Ethical and accessibility notes on using regularised logistic regression in sensitive domains and designing colour‑blind‑friendly visualisations.

## Repository structure

- `notebooks’: ’logreg_regularization_2d.ipynb’  
  Jupyter notebook with all experiments, figures, and explanations. Running this notebook from top to bottom reproduces every plot used in the tutorial.

- `report’: ‘logreg_regularization_tutorial.pdf`  
  Short written tutorial (under 2000 words) explaining the method, experiments, results, ethical considerations, and practical guidelines, with references.

- `README.md`  
  This file, giving an overview of the project and how to run it.

- `LICENSE`  
  MIT License covering reuse of the code in this repository.

## How to run the code

1. Create and activate a Python 3 environment.  
2. Install dependencies:
pip install numpy matplotlib scikit-learn

3. Open the notebook:

jupyter notebook logreg_regularization_2d.ipynb

4. Run all cells from top to bottom. This will:

- Generate the synthetic dataset.  
- Train the baseline model and a range of `C` values.  
- Produce accuracy–vs–`C` curves, decision‑boundary plots, and coefficient‑magnitude plots that match those in the report.


## Accessibility notes

Plots use a colour‑blind‑friendly Matplotlib style and combine colour with marker shapes and clear legends, following common accessibility guidance.Axis labels and titles describe the meaning of each figure (for example “Accuracy vs C” or “Effect of L2 regularization on coefficient magnitudes”), and the report includes concise alt text for every figure so that screen‑reader users can follow the main ideas.

## References

Key sources used to prepare this tutorial include the scikit‑learn documentation for `LogisticRegression` and `make_classification`, introductory articles on logistic regression and regularization, and guidance on accessible colour use in data visualisation.


