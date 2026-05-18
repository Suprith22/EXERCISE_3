# Brain Tumor Classification using XGBoost

## Overview

This project implements multiple XGBoost-based approaches for brain tumor MRI classification.

Implemented methods:

* Raw XGBoost
* PCA + XGBoost
* VGG16 + XGBoost

---

## Methodology

### Raw XGBoost

Pipeline:
Image → Resize → Flatten → XGBoost

Raw image pixel values were directly used for classification.

---

### PCA + XGBoost

Pipeline:
Image → Flatten → PCA → XGBoost

PCA was used to reduce feature dimensionality before classification.

---

### VGG16 + XGBoost

Pipeline:
Image → VGG16 Feature Extraction → XGBoost

A pretrained VGG16 CNN model was used for deep feature extraction before XGBoost classification.

---

## Important Concepts

* XGBoost
* Ensemble Learning
* Gradient Boosting
* PCA
* Deep Feature Extraction
* Transfer Learning
* Medical Image Classification

---

## Evaluation Metrics

* Accuracy
* F1-score
* Sensitivity
* Specificity

---

## Observations

* VGG16 + XGBoost achieved strong performance because pretrained CNN features captured important medical image patterns.

* PCA reduced dimensionality but sometimes removed useful information important for classification.

* Raw XGBoost preserved more original image information than PCA + XGBoost in some cases.

