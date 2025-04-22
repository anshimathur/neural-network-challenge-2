# Predicting Employee Attrition and Department Classification Using TensorFlow

## 📌 Goal

The goal of this project is to build a multi-output neural network model using TensorFlow and Keras to:
1. Predict **employee attrition** (whether an employee will leave the company).
2. Classify the **employee's department** based on given features.

By solving this, companies can proactively take action to retain employees and better understand departmental trends within their workforce.

---

## ❓ Problem Statement

Employee attrition poses a serious cost and talent management issue to organizations. Additionally, accurately categorizing departments based on various employee features can aid in organizational planning and HR analytics. This project tackles a multi-output problem where the model must learn to simultaneously handle:
- **Binary classification** (attrition: yes/no)
- **Multi-class classification** (department category)

---

## ⚙️ Model Overview

We used a Functional API in TensorFlow/Keras to build a model with:
- Shared input layers
- Two output layers:
  - A `sigmoid`-activated output for binary attrition prediction
  - A `softmax`-activated output for multi-class department classification

Training was done over 20 epochs with a batch size of 32, and 20% of the training data was used for validation.

---

## 📈 Accuracy Scores

- **Attrition Prediction Accuracy**: `0.8696`
- **Department Classification Accuracy**: `0.7011`

These results show strong performance in identifying whether an employee is likely to leave, while also maintaining a reasonable prediction rate for department classification.

---

## 🌟 Unique or Interesting Observations

- Attrition data appeared to be imbalanced, with significantly fewer employees leaving than staying. Despite this, the model performed well, possibly aided by the shared representations learned across tasks.
- Department classification was slightly more challenging, potentially due to overlapping feature characteristics between different departments.
- Using a multi-output model allowed for more efficient training by sharing intermediate representations.

---
