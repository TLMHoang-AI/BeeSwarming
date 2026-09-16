# Dataset Notes

The research uses two bee-audio datasets, referred to as **SB1 (Swarming Bee sound 1)** and **SB2 (Swarming Bee sound 2)**. The raw audio is intentionally not distributed through this public repository.

## SB1

SB1 is intended to stress generalization. Training, validation, and test data are separated using three main factors:

- data collection time,
- recording location,
- swarming state.

This split design reduces overlap between the conditions seen during training and those used for evaluation. SB1 recordings are described in the original project notes as using a 16 kHz sampling rate.

## SB2

SB2 is designed around greater recording diversity. Its samples include variation across collection days and recording devices while maintaining independent training, validation, and test partitions. The original project notes describe SB2 recordings as using a 32 kHz sampling rate.

## Purpose of the Two-Dataset Evaluation

The two datasets therefore emphasize different aspects of the study:

- **SB1:** robustness to meaningfully unseen acquisition conditions.
- **SB2:** adaptability to broader recording diversity.

The experiment notebooks preserve the preprocessing and model-training strategies used for each dataset, but the underlying audio files are not part of this repository.
