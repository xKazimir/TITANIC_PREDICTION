# Titanic Survival Prediction

**Project Description**  
This repository contains an end-to-end machine learning pipeline to predict which passengers survived the sinking of the Titanic. It covers data loading, exploratory analysis, preprocessing, feature engineering, model training, evaluation, and prediction.  

This work is based on the YouTube tutorial **“Titanic Survival Prediction in Python – Machine Learning Project”** (published ~3.4 years ago)
(https://www.youtube.com/watch?v=fATVVQfFyU0)
and implements the original Kaggle competition **“Titanic – Machine Learning from Disaster”** https://www.kaggle.com/c/titanic/overview.

---

## Table of Contents
- [Dataset](#dataset)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Modeling](#modeling)  
- [Results](#results)
  
---

## Dataset  
The data comes directly from the Kaggle competition and consists of two files:  
- **train.csv** (891 samples, with labels)  
- **test.csv** (418 samples, without labels)  

You can download them here: https://www.kaggle.com/competitions/titanic/data.

---

## Installation  
1. **Clone the repository**  
   ```bash
   git clone https://github.com/<your-username>/titanic-survival-prediction.git
   cd titanic-survival-prediction
    ```
2. **Create & activate a virtual environment**
  ```bash
python3 -m venv venv
source venv/bin/activate
  ```
3. **Install dependencies**
  ```bash
pip install -r requirements.txt
   ```

---

## Usage
Open jupyter notebook in terminal
```bash
jupyter notebook
```
Run all the cells

## Modeling

We evaluated several classifiers using cross-validated grid search:

- **Logistic Regression**  
- **Decision Tree**  
- **Random Forest**  
- **Gradient Boosting**

All hyperparameters were tuned via `GridSearchCV` on the training set.  

## Results
After submitting to the kaggle challenge, the model scored about 78% score.

