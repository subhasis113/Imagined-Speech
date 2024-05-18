# Imagined-Speech
This project classifies imagined speech with a focus on vowel articulation using EEG data. It involves preprocessing, feature extraction with discrete wavelet transform, and classification via an AutoEncoder and a Siamese Network with Triplet Loss, advancing voice recognition and neuroinformatics.

## Project Overview

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Preprocessing](#preprocessing)
- [Feature Extraction](#feature-extraction)
- [Methodology](#methodology)
- [Model Architecture](#model-architecture)
- [Results](#results)

## Introduction

This project focuses on classifying imagined speech signals with an emphasis on vowel articulation using EEG data. The main objectives are:
1. Implement an open-access EEG signal database recorded during imagined speech.
2. Preprocess and normalize the EEG data.
3. Extract discriminative features using discrete wavelet transform.
4. Classify the imagined speech using an AutoEncoder and enhance classification accuracy using a Siamese Network with Triplet Loss.
5. Compare the performance with a baseline Neural Network model.

## Dataset

The dataset consists of EEG signals recorded from subjects imagining speech, specifically focusing on vowel articulation. The data is divided into smaller files corresponding to individual vowels for detailed analysis and processing.

## Preprocessing

Preprocessing steps include:
- **Normalization**: Using the max-min technique to normalize the EEG data.
- **Artifact Removal**: Ensuring the quality of the EEG signals by removing noise and artifacts.

## Feature Extraction

To enhance discriminative features, the discrete wavelet transform is applied to the preprocessed EEG data. This step is crucial for extracting relevant features that improve classification performance.

## Methodology

### AutoEncoder-based Classification

An AutoEncoder is used for initial classification of the imagined speech signals. This neural network model learns an efficient representation of the data by encoding and decoding the input signals.

### Siamese Network with Triplet Loss

To further enhance the classification accuracy, a Siamese Network with Triplet Loss is implemented. This network architecture improves the model's ability to differentiate between different classes by learning the relative distances between the input samples.

### Comparative Analysis

For comparative analysis, a baseline model using standard Neural Networks is developed. This helps in evaluating the effectiveness of the advanced models used in this study.

## Model Architecture

The project involves two main models:
1. **AutoEncoder**: For initial classification.
2. **Siamese Network with Triplet Loss**: For enhanced classification accuracy.

The AutoEncoder model includes:
- Input Layer
- Encoder: Several layers reducing dimensionality
- Decoder: Several layers reconstructing the input
- Output Layer

The Siamese Network includes:
- Twin networks sharing weights
- Triplet Loss function to optimize relative distances between inputs

## Results

The models were trained and evaluated on the preprocessed dataset. The Siamese Network with Triplet Loss demonstrated improved classification accuracy compared to the baseline Neural Network model.
