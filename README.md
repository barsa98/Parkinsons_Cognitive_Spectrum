# Cognitive Status Classification in Parkinson’s Disease using Structural MRI
Overview
This repository presents a comprehensive machine learning–based framework to classify Parkinson’s Disease (PD) and its cognitive subtypes using T1-weighted structural MRI data.
The study focuses on distinguishing between healthy controls and Parkinson’s disease patients with varying cognitive status, while emphasizing robust validation and model interpretability.

#Objectives

To classify Parkinson’s Disease and its cognitive subtypes using structural MRI–derived features

To evaluate multiple classification models using stratified cross-validation and nested cross-validation

To provide model interpretability using SHAP (SHapley Additive exPlanations)

To identify neuroanatomical features contributing to cognitive impairment in PD

#Classification Tasks

The following classification problems were investigated:

Healthy Control (HC) vs Parkinson’s Disease (PD)

Healthy Control (HC) vs PD with Normal Cognition (PD-NC)

Healthy Control (HC) vs PD with Mild Cognitive Impairment (PD-MCI)

PD-NC vs PD-MCI

Multiclass Classification: HC vs PD-NC vs PD-MCI

# Dataset Information

Title: Resting State MRI data from healthy control (HC), Parkinson's disease with normal cognition (PD-NC), and Parkinson's disease with mild cognitive impairment (PD-MCI) cohorts

Description: This dataset is part of a longitudinal study investigating Parkinson’s Disease (PD) and its associated cognitive impairments. Resting-state MRI data were collected from:

Healthy Controls (HC):

Parkinson’s Disease patients with normal cognition (PD-NC):

Parkinson’s Disease patients with mild cognitive impairment (PD-MCI):

The dataset follows the Brain Imaging Data Structure (BIDS) specification.

# Source
OpenNeuro
🔗 https://openneuro.org/datasets/ds005892/versions/1.0.0

# Citation
Kemp, A. S., Eubank, J., Younus, Y., Galvin, J. E., Prior, F. W., & Larson-Prior, L. J. (2025).
Resting State MRI data from healthy control (HC), Parkinson's disease with normal cognition (PD-NC), and Parkinson's disease with mild cognitive impairment (PD-MCI) cohorts.
OpenNeuro. https://doi.org/10.18112/openneuro.ds005892.v1.0.0

Neuroimaging Modality: T1-weighted structural MRI

# Preprocessing & Feature Extraction

Segmentation software: FreeSurfer v7.4.1

Cortical and subcortical features were extracted from T1-weighted MRI scans

Features were used as inputs for downstream machine learning models

# Machine Learning Models

The following classification models were evaluated:

Logistic Regression

Support Vector Machine (RBF kernel)

K-Nearest Neighbors (KNN)

Decision Tree

Random Forest

Gradient Boosting

Bagging Classifier

Voting Classifier (ensemble)

# Validation Strategy

Stratified K-Fold Cross-Validation for performance estimation

Nested Cross-Validation for unbiased hyperparameter tuning and evaluation

Performance metric: ROC-AUC

Model Interpretability

SHAP (SHapley Additive exPlanations) was used to:

Quantify feature importance

Visualize feature contributions using bar plots and beeswarm plots

A PDF report is included containing:

SHAP visualizations

Detailed interpretation of important neuroanatomical features

#Outputs

ROC curves for each fold and classification task

Mean and standard deviation of ROC-AUC scores

SHAP-based feature importance plots

Interpretable insights into brain regions associated with cognitive decline in PD
