# Scienta_project

## Classification of healthy, RA and SLE patients using machine learning on transcriptomics data

## Description

This project consists of three scripts that utilize transcriptomics data from datasets of healthy, RA (Rheumatoid Arthritis), and SLE (Systemic Lupus Erythematosus) patients to build a machine learning model for disease classification. The model is also analyzed to identify the genes that drive classification, which may serve as potential biomarkers for each disease. Each script is briefly described in the following sections.

## Script 1: Data Exploration

Objective: Understand the available datasets and identify differences, key features, and any possible inconsistencies.

Steps:

    Examine data structure and format: Check whether files are consistent in terms of columns and data types (e.g., normalized or raw values).
    Descriptive statistics: Analyze the means and distributions of expression levels across datasets.
    Identify missing values and outliers: Note any outliers and assess how each dataset is impacted.

## Script 2: Data Preprocessing

Objective: Standardize the data to enable consistent use in the model.

Steps:

    Gene filtering: Select genes that are common across datasets to reduce bias from genes absent in some datasets.
    Data transformation:
        Normalization: Apply log1p normalization to make expression levels comparable across individuals and datasets.
        Batch Effect Correction: Use batch effect correction methods to address measurement differences between datasets.
    Variable gene selection: Retain only the most variable genes to simplify the model and avoid overfitting.

## Script 3: Classification

Objective: Train an effective classification model for the task of distinguishing RA, SLE, and healthy individuals.

Models used:

    Random Forest
    Deep Neural Networks

Performance Evaluation: Model performance is assessed using accuracy and F1-score on previously unseen test datasets.

Additionally, a feature importance analysis is conducted to identify genes that significantly contribute to the model’s predictions as potential "drivers" of each disease.


