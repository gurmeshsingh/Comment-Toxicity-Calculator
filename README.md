# Comment-Toxicity-Calculator

This repository contains a machine learning pipeline to detect and classify toxic comments into multiple categories using Natural Language Processing (NLP). It was developed using the dataset from the [Kaggle Jigsaw Toxic Comment Classification Challenge](https://www.kaggle.com/competitions/jigsaw-toxic-comment-classification-challenge).

## 📌 Project Summary

This project tackles the challenge of identifying and categorizing online toxic comments. Each comment can be tagged with one or more labels from the following:
- `toxic`
- `severe_toxic`
- `obscene`
- `threat`
- `insult`
- `identity_hate`

The model is built using:
- Text preprocessing & cleaning
- TF-IDF vectorization
- Multi-label classification (Logistic Regression)
- Evaluation using ROC-AUC
- Submission output formatted for Kaggle

---
