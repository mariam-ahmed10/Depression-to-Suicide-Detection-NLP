# Depression-to-Suicide-Detection-NLP

## Overview

This project investigates whether machine learning and NLP models trained on depression-related social media content can generalize to suicidal intention detection across different domains.

The study evaluates the effectiveness of traditional feature-based approaches and transformer-based language models for cross-domain mental health classification.

---

## Problem Statement

Mental health datasets are often collected from different sources and domains. Models trained on one domain may struggle when applied to another.

This project explores whether knowledge learned from depression-related content can transfer to suicidal intention detection tasks.

---

## Datasets

### Training Domain

* Depression Detection Dataset (MDDL)

### Evaluation Domain

* Twitter Suicidal Intention Dataset

---

## Methodology

Three feature representation approaches were evaluated:

### Experiment A

* TF-IDF Features

### Experiment B

* RoBERTa Embeddings

### Experiment C

* MentalBERT Embeddings

The generated features were evaluated using multiple classifiers including:

* Naive Bayes
* Random Forest
* Decision Tree
* SVM
* Logistic Regression
* K-Nearest Neighbors (KNN)

---

## Key Findings

### Best Cross-Domain Model

RoBERTa + KNN

Performance:

* F1 Score: 0.6447
* Recall: 0.5429
* Accuracy: 0.8125

### Major Research Insight

KNN achieved the worst performance when using TF-IDF features (F1 = 0.0009).

However, when using RoBERTa embeddings, KNN became the best-performing model (F1 = 0.6447).

This demonstrates that feature representation quality has a greater impact than classifier selection in cross-domain NLP transfer learning.

---

## Technologies Used

* Python
* NLP
* TF-IDF
* RoBERTa
* MentalBERT
* Scikit-Learn
* Transfer Learning
* Text Classification

---

## Repository Structure

```text
paper/
datasets/
README.md
```

---

## Research Paper

The complete project report and experimental analysis are included in the paper directory.

---

## Authors

King Saud University

Information Technology Department

Artificial Intelligence Track
