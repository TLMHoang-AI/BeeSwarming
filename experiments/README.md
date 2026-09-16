# Experiment Map

This directory preserves the research notebooks while giving them a cleaner structure for navigation.

## Feature extraction

`feature_extraction/` contains experiments that transform raw bee audio into handcrafted acoustic representations:

- `mfcc/` — MFCC extraction for SB1/SB2
- `stft/` — STFT-based spectral extraction
- `chroma/` — Chroma feature extraction
- `combined/` — paired and multi-feature extraction experiments
- `extract_all_features.ipynb` — consolidated MFCC + STFT + Chroma extraction workflow

## Model training

`model_training/` contains classifier training and hyperparameter-tuning notebooks grouped by feature family. Where the original experiments were dataset-specific, the notebooks are further separated into `sb1/` and `sb2/`.

## Feature selection

`feature_selection/` contains experiments that reduce or select handcrafted features before model fitting, including correlation-based and summary-statistic variants.

## Archive

`archive/` contains notebooks that were explicitly marked as old, superseded, or exact duplicates in the original repository. They are retained for research history but are not part of the primary experiment path.

## Note on execution

These notebooks were developed in the original local research environment and some contain historical absolute paths. The raw datasets are private, so this repository is intended to document methodology and experiment design rather than provide a turnkey execution package.
