# Titanic Dataset - Data Cleaning & Preprocessing

## Overview
This repository contains the data cleaning and preprocessing steps performed on the Titanic dataset as per Task 1 instructions.

## Steps Performed
1. Loaded the Titanic dataset (891 rows, 12 columns).
2. Dropped the `Cabin` column due to high missing values.
3. Handled missing values:
   - Age = filled with median
   - Embarked = filled with mode
   - Fare = filled with median
4. Encoded categorical features:
   - Sex = label encoded (male=1, female=0)
   - Embarked = one-hot encoded
5. Scaled numerical features (Age, Fare) using StandardScaler.
6. Outlier detection & removal:
   - Used IQR method on Age and Fare.
   - Final dataset: 718 rows, 14 columns.

## Files
- `Titanic-Dataset.csv`: Original dataset
- `titanic_cleaned.csv`: Final cleaned dataset
- `Task1_Titanic_Preprocessing.ipynb`: Jupyter notebook with full code
- `Task1_Report.pdf`: One-page report with summary & visuals

## How to Run
1. Open `Task1_Titanic_Preprocessing.ipynb` in Jupyter Notebook / JupyterLab / VSCode. Ensure the dataset is there. If not working then please download in from here(I have addded).
2. Run all cells to reproduce preprocessing steps.
