# Brain Tumor Classification using Hybrid VGG16-EfficientNetB0 with SE Attention

## Overview

This project presents a hybrid deep learning framework for multiclass brain tumor classification from MRI images. The proposed architecture combines VGG16 and EfficientNetB0 feature extractors with Squeeze-and-Excitation (SE) attention mechanisms to improve feature representation and classification performance.

The model classifies MRI scans into four categories:

- Glioma
- Meningioma
- Pituitary Tumor
- No Tumor

## Key Features

- Hybrid VGG16 + EfficientNetB0 Architecture
- Squeeze-and-Excitation (SE) Attention
- Dual Pooling (Global Average Pooling + Global Max Pooling)
- Transfer Learning with Fine-Tuning
- Batch Normalization and Dropout Regularization
- Label Smoothing
- Grad-CAM Explainability
- ROC Curve Analysis
- Confusion Matrix Evaluation

## Dataset

Dataset Source:
https://drive.google.com/file/d/1OPUSnue5Kj0jjgOnSmE4Cbzu9jYztZJG/view?usp=drive_link

Classes:
- Glioma
- Meningioma
- Pituitary
- No Tumor

Input Image Size: 224 × 224 × 3

## Model Architecture

- Backbone 1: VGG16
- Backbone 2: EfficientNetB0
- SE Attention Module
- Feature Fusion Layer
- Dense (512)
- Dense (256)
- Dense (128)
- Softmax Output Layer

## Training Configuration

| Parameter | Value |
|------------|---------|
| Image Size | 224×224 |
| Batch Size | 32 |
| Optimizer | Adam |
| Loss Function | Categorical Crossentropy |
| Label Smoothing | 0.05 |
| Fine-Tuning | Enabled |

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix
- Grad-CAM Visualization

## Results

The proposed hybrid model achieved excellent performance in four-class brain tumor classification and demonstrated strong generalization capability on unseen MRI images.

## Grad-CAM Explainability

Grad-CAM visualization highlights the tumor-relevant regions used by the model for prediction, providing better interpretability and clinical trustworthiness.


```

## Author

akila ibnath
