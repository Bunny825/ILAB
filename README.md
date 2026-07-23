# ILAB CARE — Integrated Disease Prediction System

A multi-disease clinical screening application that predicts the likelihood of several conditions
and estimates medical expenses from patient inputs — combining classical machine-learning and
deep-learning models behind a single interface.

> **Published at the ICIEMS 2025 International Conference.**

## What It Predicts

| Module | Model |
|---|---|
| Heart Disease | scikit-learn |
| Diabetes | scikit-learn |
| Parkinson's Disease | scikit-learn |
| Cardiovascular Disease | Deep learning (Keras) |
| Medical Expense Estimation | Deep-learning regression (Keras) |

## Tech Stack

- **scikit-learn** — trained classifiers with saved models + scalers (`.sav`)
- **TensorFlow / Keras** — deep-learning models (`.h5`)
- **Streamlit** + `streamlit-option-menu` — multi-module UI
- **NumPy**

## How It Works

Each condition has its own trained model and feature scaler. The app collects the relevant clinical
inputs, scales them consistently with training, runs the appropriate model, and returns a prediction
(or, for the expenses module, an estimated cost). The training datasets are included in the
repository.

## Getting Started

```bash
pip install -r requirements.txt
streamlit run multiple_disease_prediction.py
```

Select a module from the sidebar, enter the clinical values, and get a prediction.

## Research

This work was published at the **ICIEMS 2025 International Conference** as part of the ILAB CARE
project.
