# Loan Dataset Exploration: Probability of Default and Loss Given Default Models

This project explores a loan dataset and builds two key models in credit risk modeling:
1. **Probability of Default (PD)** model: Uses fine and coarse classing techniques, Weight of Evidence (WoE) transformation, and logistic regression to predict the likelihood of default.
2. **Loss Given Default (LGD)** model: Utilizes Fannie Mae dataset (2003–2013) with intensive feature engineering and models loss severity using regression techniques and XGBoost.

## Project Overview

This project focuses on the following:
1. **Probability of Default (PD)**:
   - Preprocessing loan data using fine and coarse classing techniques.
   - Calculating Weight of Evidence (WoE) for discrete and continuous variables.
   - Building a logistic regression model to predict default likelihood.

2. **Loss Given Default (LGD)**:
   - Working with Fannie Mae historical mortgage data (2002–2018) with about 550K delinquent loans.
   - Intensive feature engineering, including transformations for categorical and continuous variables.
   - Predicting LGD using regression and XGBoost models.

---

## Project Structure

```plaintext
/Loan_Risk_Modeling_Project
    ├── data/
    │   ├── loan_data_train.csv           # Preprocessed training data
    │   ├── loan_data_test.csv            # Preprocessed test data
    │   ├── loan_data_label_train.csv     # Training labels
    │   ├── loan_data_label_test.csv      # Test labels
    ├── notebooks/
    │   ├── PD_model.ipynb                # Notebook for Probability of Default (PD) model
    │   ├── loan_data_PD_proj.ipynb       # Data preprocessing notebook for PD model
    │   ├── LGD_model.ipynb               # Notebook for Loss Given Default (LGD) model
    ├── images/
    │   ├── feature_importance.png        # Visualization of feature importance

```
## PD Preprocessing

The preprocessing notebook (`loan_data_PD_proj.ipynb`) contains steps for:
1. **Handling Missing Data**: Imputation of missing values.
2. **Feature Engineering**:
   - **Fine and Coarse Classing**: Binning continuous features into categories.
   - **Weight of Evidence (WoE)**: Calculating WoE for both categorical and continuous features.
3. **Train-Test Split**: Saving the preprocessed training and test datasets.


## PD Modeling

The modeling notebook (`PD_model.ipynb`) focuses on:
1. **Logistic Regression**: Using the WoE-transformed features to build a logistic regression model.
2. **Model Evaluation**: Performance evaluation using metrics like accuracy, ROC-AUC, and confusion matrices.
3. **Feature Importance**: Analysis of important variables in default prediction.

**Open the notebooks**:
   you can open the notebooks in Jupyter and execute the cells to preprocess data and train the model interactively.
   This will train the logistic regression model and output performance metrics like AUC and confusion matrix.

## References

- **Weight of Evidence (WoE)**: A statistical method commonly used in credit scoring.
- **Logistic Regression**: A popular technique for binary classification tasks.
