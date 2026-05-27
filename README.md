# EfficientNet-Based Multi-Class Brain Tumor MRI Classification

This repository contains the implementation used for the study:

**"EfficientNet Architectures for Multi-Class Brain Tumor Classification Using MRI"**

## Overview

This study evaluates the complete EfficientNet family (B0–B7 and EfficientNetV2) for multi-class brain tumor classification using T1-weighted contrast-enhanced MRI.

The framework includes:

- Two-phase transfer learning
- MRI-specific preprocessing
- Data augmentation
- Label smoothing
- Cosine annealing learning-rate scheduling
- Cross-validation
- Grad-CAM explainability

## Dataset

The dataset used in this study is:

**BrainTumorMRIDataset (Kaggle)**

## Repository Contents

- EfficientNetB0.ipynb
- EfficientNetB1_B2.ipynb
- EfficientNetB3_B4.ipynb
- EfficientNetB5.ipynb
- EfficientNetB6.ipynb
- EfficientNetB7.ipynb
- EfficientNetV2.ipynb

## Experimental Setup

Training followed a two-phase transfer learning strategy:

### Phase 1
- Frozen backbone
- Adam optimizer
- 10 epochs

### Phase 2
- Full fine-tuning
- SGD with momentum
- Cosine annealing
- 20 epochs

## Reproducibility

This repository contains training and evaluation scripts used in the manuscript to improve transparency and reproducibility.
