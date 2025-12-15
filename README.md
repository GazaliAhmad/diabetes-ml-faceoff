
# Model Selection Under Constraint

## Project Overview

This project is a case study in model selection under constraint. The objective was not to identify the most accurate model, but to examine how different machine learning approaches behave when data is limited, ambiguous, and partially unreliable.

The dataset used is intentionally small and noisy, reflecting common real-world conditions where analytical judgement matters more than algorithmic sophistication.

This repository documents the reasoning behind selecting one model as fit-for-purpose, and rejecting others that appeared statistically attractive but posed interpretability or stability risks.

![Python](https://img.shields.io/badge/Python-3.11-blue) ![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange) ![Status](https://img.shields.io/badge/Status-Complete-green)

---

## Context

In many applied settings, especially outside of large technology firms, data quality and quantity are the primary constraints. Models that perform well numerically can still be unsuitable if they are difficult to interpret, unstable under small samples, or prone to misleading confidence.

This project treats model selection as a **risk decision**, not a leaderboard exercise.

---

## Models Evaluated

Two modelling approaches were evaluated:

- **Polynomial Logistic Regression**  
  Chosen as an interpretable baseline with transparent coefficients and predictable behaviour.

- **Random Forest Classifier**  
  Evaluated for its ability to capture non-linear interactions, at the cost of interpretability and stability.

Models were assessed neutrally, without anthropomorphic or competitive framing.

---

## Decision Criteria

Model selection was guided by the following criteria:

- Interpretability of outputs  
- Stability under small-sample conditions  
- Susceptibility to overfitting  
- Risk of misleading confidence  

Predictive accuracy was considered contextual information, not a decisive metric.

---

## Observations (Contextual Metrics)

Observed accuracy values are presented for context only. They informed understanding of model behaviour but were not used as the primary decision driver.

| Criterion | Logistic Regression | Random Forest |
|--------|---------------------|---------------|
| Interpretability | High | Low |
| Stability | High | Medium |
| Risk of overconfidence | Low | High |
| Observed accuracy (contextual) | Lower | Higher |

---

## Decision Outcome

Although the Random Forest model showed higher observed accuracy in this dataset, it was not selected due to interpretability limitations and instability under the given data constraints.

The Logistic Regression model was selected as fit-for-purpose, as it provided clearer insight, more stable behaviour, and lower epistemic risk in this context.

---

## What This Project Does Not Claim

- This is not a medical or clinical diagnostic tool  
- This does not claim causal inference  
- This does not argue that higher accuracy is undesirable  
- This does not generalise beyond the dataset and constraints examined  

The purpose of this project is to demonstrate **decision reasoning**, not predictive superiority.

---

## Key Takeaway

In constrained data environments, the least misleading model is often more valuable than the most accurate one.

Model selection is not purely a technical optimisation problem. It is a judgement call under uncertainty.
