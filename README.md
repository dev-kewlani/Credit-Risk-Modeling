# Loan Dataset Exploration and Probability of Default Model

This project explores a loan dataset and builds a Probability of Default (PD) model using fine and coarse classing techniques, WoE transformation, and logistic regression. The goal is to preprocess loan data, calculate the Weight of Evidence (WoE) for discrete and continuous variables, and build a robust model for default prediction.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Project Structure](#project-structure)
3. [Preprocessing](#preprocessing)
4. [Modeling](#modeling)
5. [Dependencies](#dependencies)
6. [How to Run](#how-to-run)
7. [References](#references)

## Project Overview

In this project, we:
- Preprocess the loan dataset using fine and coarse classing techniques.
- Calculate Weight of Evidence (WoE) for various features.
- Use these WoE-transformed features to build a Probability of Default (PD) model with logistic regression.
- Split the data into training and test sets to validate the model.

## Project Structure

```plaintext
/Loan_PD_Model_Project
    ├── data/
    │   ├── loan_data_train.csv       # Preprocessed training data
    │   ├── loan_data_test.csv        # Preprocessed test data
    │   ├── loan_data_label_train.csv # Training labels
    │   ├── loan_data_label_test.csv  # Test labels
    ├── notebooks/
    │   ├── PD_model.ipynb            # Full notebook for building the PD model
    │   ├── loan_data_PD_proj.ipynb   # Data preprocessing notebook
    ├── scripts/
    │   ├── preprocess.py             # Script to preprocess the data
    │   ├── model.py                  # Script to build and evaluate the model
    ├── README.md                     # Project description and instructions
    ├── requirements.txt              # Python dependencies
