# Chest X-ray Classification using XGBoost

## Overview

This project implements multiple XGBoost-based approaches for pneumonia detection using chest X-ray images.

Implemented methods:

* Raw XGBoost
* PCA + XGBoost
* VGG16 + XGBoost

---

## Methodology

### Raw XGBoost

Pipeline:
Image → Resize → Flatten → XGBoost

Raw image pixel values were directly used as input features for XGBoost classification.

---

### PCA + XGBoost

Pipeline:
Image → Flatten → PCA → XGBoost

PCA was used for dimensionality reduction before classification.

---

### VGG16 + XGBoost

Pipeline:
Image → VGG16 Feature Extraction → XGBoost

A pretrained VGG16 CNN model was used as a deep feature extractor. Extracted features were flattened and given to XGBoost for classification.

---

## Important Concepts

* XGBoost
* Gradient Boosting
* PCA Dimensionality Reduction
* Transfer Learning
* Deep Feature Extraction
* Medical Image Classification

---

## Evaluation Metrics

* Accuracy
* F1-score
* Sensitivity
* Specificity

---

## Observations

* VGG16 + XGBoost achieved better performance because deep CNN features captured richer image representations.

* Raw XGBoost performed better than PCA + XGBoost, suggesting that PCA removed some useful discriminative information.

* Deep feature extraction significantly improved classification performance compared to using raw pixels directly.

