# Titanic Survival Prediction

This project is a classic beginner-friendly machine learning task that uses data from the Titanic disaster to predict which passengers survived.

## Overview

- *Goal*: Predict whether a passenger survived the Titanic disaster.
- *Algorithm Used*: Random Forest Classifier
- *Final Accuracy: **82.6%*

---

## Dataset

- Source: [Kaggle Titanic Dataset](https://www.kaggle.com/competitions/titanic/data)
- Files:
  - Titanic.csv
- Target Column: Survived (0 = Did not survive, 1 = Survived)

---

## Features Used

- Pclass (Ticket class)
- Sex (Gender)
- Age
- SibSp (Siblings/Spouses aboard)
- Parch (Parents/Children aboard)
- Fare
- Embarked (Port of Embarkation)

---

## Workflow

1. *Data Cleaning*
   - Handled missing values in Age, Embarked
   - Dropped irrelevant columns: Name, Ticket, Cabin

2. *Feature Encoding*
   - Converted categorical features like Sex, Embarked into numerical values

3. *Model Training*
   - Split data into training and validation sets
   - Used RandomForestClassifier from sklearn
   - Tuned hyperparameters for better performance

4. *Model Evaluation*
   - Accuracy on validation set: *82.6%*
   - Used confusion matrix and classification report

5. *Model Saving*
   - Exported trained model using joblib as titanic_model.pkl

---

## How to Run

1. Clone this repo
2. Install required packages:
   ```bash
   pip install -r requirements.txt
