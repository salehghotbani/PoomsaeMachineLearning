[![Python](https://img.shields.io/badge/Python%203.11-red?logo=python&logoColor=fff)](#)
[![CUDA](https://img.shields.io/badge/CUDA_Toolkit-12.8-blue)](#)
[![cuDNN](https://img.shields.io/badge/cuDNN-9.8.0-blue)](#)
[![RFDETR](https://img.shields.io/badge/RFDETR-1.2.1-blue)](#)
[![RTMO](https://img.shields.io/badge/RTMO-0.0.14-blue)](#)

# Pose-Based Taekwondo Poomsae Recognition with SVM and Logistic Regression

This repository contains the full pipeline for pose-based recognition of Taekwondo Poomsae forms using geometric normalization and classical machine learning classifiers.

The work focuses on analyzing the impact of translation and scale normalization on pose-derived features.

## Pipeline Overview

1. Human detection (RF-DETR)
2. Multi-person tracking (ByteTrack)
3. Pose estimation (RTMO)
4. Frame sampling (stride=4)
5. Geometric normalization
6. Feature extraction (mean pooling)
7. Classification (Logistic Regression, SVM)
8. Evaluation metrics and confusion matrix

## Dataset

The processed pose dataset is publicly available via Zenodo:

DOI: 

Raw videos are NOT distributed due to licensing constraints. Only pose keypoints and derived features are released.

## Installation

`pip install -r requirements.txt`

## Normalization Methods

- Translation normalization (nose-centered)
- Scale normalization (shoulder-hip distance)
- Combined normalization

## Metrics

Accuracy, Precision, Recall, F1-score, Confusion Matrix

## License

MIT License


## Citation

If you use this code, please cite:

(put paper citation later)
