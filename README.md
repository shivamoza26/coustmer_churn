# Customer Churn Prediction

Machine learning project for exploring and predicting telecom customer churn using the Telco Customer Churn dataset.

## Project Overview

This repository contains:
- Exploratory data analysis (EDA) in notebooks
- Model training and testing workflow
- Pre-split train and test data files

Goal: build and evaluate churn prediction models to identify customers likely to leave.

## Repository Structure

```text
main.py
pyproject.toml
README.md
code/
	eda.ipynb
	modeltrainingtesting.ipynb
data/
	Telco-Customer-Churn.csv
new data/
	x_test
	x_train
	y_test
	y_train
```

## Dataset

- Source file: `data/Telco-Customer-Churn.csv`
- Target variable: `Churn`

## Environment Setup

This project uses a local virtual environment (`.venv`) and dependencies from `pyproject.toml`.

1. Create and activate a virtual environment (if not already done):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2. Install dependencies:

```powershell
pip install -e .
```

If editable install is not configured in your environment, install required packages directly with `pip`.

## How To Run

### Option 1: Notebook Workflow (recommended)

1. Open `code/eda.ipynb` for data exploration and preprocessing review.
2. Open `code/modeltrainingtesting.ipynb` for model building and evaluation.
3. Run cells in order.

### Option 2: Python Script

If `main.py` is configured for your current workflow, run:

```powershell
python main.py
```

## Typical ML Workflow In This Project

1. Load telecom churn data
2. Clean and preprocess features
3. Split train/test data
4. Train classification models
5. Evaluate performance using classification metrics

## Notes

- Folder name `new data/` includes a space; keep the exact path when loading files.
- Repository default branch on GitHub is `main`, while current local branch is `master`.

