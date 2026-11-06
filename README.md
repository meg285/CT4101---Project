# Predicting Student Exam Performance Using Machine Learning

## Project Overview

This project was developed for CT4101 Machine Learning at the University of Galway.  

The aim is to predict students final mathematics grades using machine learning.

Three regression moels are compared:
1. Baseline Model (Dummy Regressor)
2. Linear Regression
3. Decision Tree Regression


## Dataset

The project uses the Student Performance dataset from the UCI Machine Learning Repository.
The dataset contains information about 395 students studying maths in Portuguese secondary schools.

The following features are used:
- studytime: weekly study time category
- absences: number of school absences
- G1: first-period maths grade
- G2: second-period maths grade

The target variable is G3, the final maths grade (0-20)

Dataset source: https://archive.ics.uci.edu/dataset/320/student+performance


## Methods

The dataset was split into 80% training data and 20% testing data.

Three regression models were evaluated using: 
- Mean Absolute Error (MSE)
- Root Mean Squared Error (RMSE)
- 5-fold cross-validation


## Results

| Model | Test MAE | Test RMSE | CV MAE |
| ----- | -------- | --------- | ------ |
| Baseline | 3.6459 | 4.5502 | 3.3883 |
| Linear Regression | 1.3126 | 2.0443 | 1.1603 |
| Decision Tree | 1.3100 | 2.1687 | 1.1735 |

Linear Regression was selected as the preferred model because of its simplicity and competitive performance


## How to Run

1. Download the project files.
2. Install the required Python libraries using:
    pip install -r requirements.txt
3. Open the Jupyter notebook
4. Run all cells in order

## Limitations

The models struggle to predict students with final grades of zero.
The dataset is relativrely small and comes from Portuguese secondary schools, so the results may not generalise to other educational settings.
The models also rely on previous grades, meaning they are most useful after first-period and second-period grades are available.

## Responsible Use

Predictions should not be used as the sole basis for decisions about students academic abilities or opportunities.

## GitHub Repository

https://github.com/meg285/CT4101---Project
