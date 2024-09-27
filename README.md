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
```

## Preprocessing

The preprocessing notebook (`loan_data_PD_proj.ipynb`) contains steps for:
1. **Handling Missing Data**: Imputation of missing values.
2. **Feature Engineering**:
   - **Fine and Coarse Classing**: Binning continuous features into categories.
   - **Weight of Evidence (WoE)**: Calculating WoE for both categorical and continuous features.
3. **Train-Test Split**: Saving the preprocessed training and test datasets.

The script `preprocess.py` performs the same operations programmatically, allowing easy and automated processing of new data.

## Modeling

The modeling notebook (`PD_model.ipynb`) focuses on:
1. **Logistic Regression**: Using the WoE-transformed features to build a logistic regression model.
2. **Model Evaluation**: Performance evaluation using metrics like accuracy, ROC-AUC, and confusion matrices.
3. **Feature Importance**: Analysis of important variables in default prediction.

The script `model.py` can be used to automate the training and evaluation process.

## Dependencies

To run this project, install the following dependencies listed in `requirements.txt`:
```plaintext
pandas
numpy
scikit-learn
matplotlib
seaborn
```

## How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your_username/Loan_PD_Model_Project.git
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the preprocessing script**:
   ```bash
   python scripts/preprocess.py
   ```
   This will generate the preprocessed data files in the `data/` directory.

4. **Run the model training script**:
   ```bash
   python scripts/model.py
   ```
   This will train the logistic regression model and output performance metrics like AUC and confusion matrix.

5. **Open the notebooks**:
   Alternatively, you can open the notebooks in Jupyter and execute the cells to preprocess data and train the model interactively.

## References

- **Weight of Evidence (WoE)**: A statistical method commonly used in credit scoring.
- **Logistic Regression**: A popular technique for binary classification tasks.
```
