# Bee Swarming Detection Using Audio Signals

This project introduces a machine learning-based system for early and accurate detection of swarming behavior in honeybee colonies using sound signals. It was developed as part of a research effort to support smart beekeeping practices through non-invasive audio analysis.

## Overview

Swarming in bee colonies is a critical event that affects productivity and stability. Traditional methods for detecting swarming, such as manual observation or temperature monitoring, are inefficient and do not scale well. This project presents an approach that leverages machine learning and ensemble learning methods to analyze sound features and classify bee behaviors as swarming or non-swarming.

The core idea is to extract meaningful audio features — such as MFCC, STFT, and Chroma — from beehive recordings and use them with various classifiers to detect swarming behavior automatically and with high precision.

## Motivation

Honeybees play a vital role in ecosystems and agriculture. The rapid decline in their population due to disease, climate factors, and poor hive management makes early detection of colony changes increasingly important. Swarming, one of the most disruptive events in a hive, must be detected early to ensure stability and productivity.

Audio signal analysis has emerged as a promising, non-invasive solution. By examining frequency patterns and harmonic changes in bee sounds, we can predict swarming behavior without disturbing the hive.

## Methodology

### Feature Extraction

We extract and combine multiple features to describe the bee audio signals:

- **MFCC (Mel Frequency Cepstral Coefficients)**: Represents the short-term power spectrum of a sound, based on human auditory perception.
- **STFT (Short-Time Fourier Transform)**: Captures frequency changes over time, suitable for detecting dynamic patterns.
- **Chroma Features**: Encodes energy distribution across pitch classes, useful for tracking tonal changes in bee sounds.

### Machine Learning Models

We trained and evaluated the following classifiers:

- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Random Forest
- Extra Trees
- Gradient Boosting
- Naïve Bayes

### Ensemble Learning Strategies

To further improve accuracy and robustness, we applied:

- Soft Voting
- Hard Voting
- Weighted Voting
- Stacking

These methods combine the strengths of individual models, especially useful in noisy and imbalanced data conditions.

## Results

Our custom feature selection and model combination approach produced highly accurate results:

| Model                      | Validation Accuracy | Test Accuracy | Best F1-score |
|---------------------------|---------------------|---------------|----------------|
| Individual Classifiers     | up to 96.42%        | 99.48%        | 99.5%+         |
| Ensemble Methods           | 97.33%              | 99.17%        | 99.6%          |
| Custom Config (SB1, SB2)   | 99.57%              | 99.60%        | 99.6%          |

These results demonstrate that combining MFCC, STFT, and Chroma features with proper learning techniques leads to highly effective detection of bee swarming behavior.

## Key Contributions

- Introduced a hybrid feature extraction method combining MFCC, STFT, and Chroma.
- Achieved state-of-the-art performance using ensemble machine learning techniques.
- Provided a scalable solution for early swarming detection to support modern beekeeping.
- Delivered strong generalization on two datasets (SB1 and SB2).

## References

- Phan et al., 2022 – Evaluation of feature extraction methods for bee audio classification.
- Truong et al., 2023 – A deep learning-based approach for bee sound identification.
- Ferrari et al., 2008 – Monitoring of swarming sounds in bee hives using STFT and spectrum analysis.
