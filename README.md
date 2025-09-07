# Heart Attack Dataset – Exploratory Data Analysis

## Overview

This project presents a thorough exploratory data analysis (EDA) of a heart‑attack dataset using Python. The goal is to examine demographic and clinical variables, clean and preprocess the data, perform statistical analyses, and create visualizations that reveal meaningful patterns. Insights obtained here can help guide further predictive modelling work.

## Dataset

The dataset consists of 14 features collected from 324 patients, along with a target label indicating heart‑attack risk (`output` = 1 for higher risk, 0 otherwise). Key columns include:

- **age** – age of the patient
- **sex** – gender (0 = female, 1 = male)
- **cp** – chest‑pain type (0 = typical angina, 1 = atypical angina, 2 = non‑anginal pain, 3 = asymptomatic)
- **trtbps** – resting blood pressure (mm Hg)
- **chol** – cholesterol level (mg/dL)
- **fbs** – fasting blood sugar > 120 mg/dL (1 = true, 0 = false)
- **restecg** – resting ECG results (0 = normal, 1 = ST‑T abnormality, 2 = left‑ventricular hypertrophy)
- **thalachh** – maximum heart rate achieved
- **exng** – exercise‑induced angina (1 = yes, 0 = no)
- **oldpeak** – ST depression induced by exercise
- **slp** – slope of the peak ST segment
- **caa** – number of major vessels (0–4)
- **thall** – thalassemia rate
- **output** – target (1 = more chance of heart attack, 0 = less chance)

The raw CSV is included as `heart.csv`.


## Features

- Removal of duplicate records and imputation of missing values (median for continuous variables, mode for categorical variables).
- Computation of descriptive statistics (mean, standard deviation, quartiles) for numerical columns.
- Visualisation of heart‑attack risk by sex, chest‑pain type, age group, fasting blood sugar level, and resting ECG results.
- Statistical tests to evaluate relationships between heart‑attack occurrence and resting blood pressure, maximum heart rate, and ST‑segment/heart‑rate ratio.
- Thoroughly documented notebook with explanations and plots.

## Requirements

- Python 3.7+
- Jupyter Notebook
- numpy
- pandas
- matplotlib
- seaborn
- scipy

Install the dependencies using `pip`:

```bash
pip install numpy pandas matplotlib seaborn scipy
```

## Results Highlights

- Females and patients with atypical or non‑anginal chest pain showed higher proportions of heart‑attack events in this dataset.
- Younger age groups (30–50) had a surprisingly higher risk compared with those in their sixties, though the trend is not strictly monotonic.
- Resting ECG abnormalities and higher exercise‑induced heart rates were strongly associated with heart‑attack risk.
- A low ST‑depression–to–heart‑rate ratio (oldpeak / thalachh) was significantly linked to heart‑attack outcomes.

Contributions are welcome! If you’d like to extend the analysis or build predictive models, feel free to open a pull request or issue.
