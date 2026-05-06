# Thyroid Disease Classification

This repository contains the final integrated Jupyter notebook for a machine learning project on **binary thyroid disease classification** using the **hypothyroid / A-thyroid dataset**.

The project examines how different preprocessing strategies and classification models affect predictive performance, with particular emphasis on:

- missing values
- class imbalance
- skewed laboratory variables such as `TSH`
- mixed feature types
- leakage-aware evaluation using pipelines and cross-validation

## Repository Content

- `Thyroid_Disease_Project.ipynb`  
  Final notebook containing the complete workflow:
  - dataset understanding
  - exploratory analysis
  - preprocessing and dataset versioning
  - model benchmarking
  - candidate selection
  - hyperparameter tuning
  - final evaluation

## Project Goal

The main goal of the project was to identify which combination of preprocessing strategy and machine learning model performs best for thyroid disease classification.

Rather than relying on a single preprocessing pipeline, the project compares multiple dataset versions and several classification algorithms in order to determine which approaches are the most effective and methodologically reliable.

## How to Run

Open and run `Thyroid_Disease_Project.ipynb` in:

- **Jupyter Notebook / JupyterLab**, or
- **Google Colab**

The notebook includes the package-installation cells required for execution.

If the dataset file is not already in the expected location, update the dataset path in the notebook before running all cells from top to bottom.

## Main Results

The main outcomes of the project were:

- preprocessing strategy had a strong effect on model performance
- feature-selection-based dataset versions performed especially well
- **Random Forest** and **Gradient Boosting** were the strongest model families during experimentation
- the best final model was **Random Forest with the `V4_SFS` dataset version**
- the best final model achieved approximately **99.87% weighted F1-score** on the held-out test set

These results suggest that careful preprocessing and leakage-aware evaluation were just as important as the choice of classifier.

## Limitations

The main limitations of the project are:

- the evaluation was performed on a single dataset
- the dataset is strongly imbalanced
- results depend on preprocessing design choices
- strong performance on this dataset does not guarantee real-world generalization
- external validation on independent patient populations would still be required before any clinical use

## Intended Use

This repository is intended for:

- academic coursework
- project review
- demonstration of an end-to-end medical machine learning workflow

It is **not** intended for direct clinical use or as a standalone diagnostic system.

## Context

This project was developed in the context of an **AI in Medicine** course assignment focused on thyroid disease classification.
