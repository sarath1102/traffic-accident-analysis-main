## Overview 
This project investigates the factors contributing to traffic accidents using a large U.S. dataset. We focus specifically on the challenge of imbalanced ordinal variables like severity levels (1 to 4). Using data mining techniques such as Random Forest, XGBoost, and LightGBM, we apply the Knowledge Discovery in Databases (KDD) methodology to uncover patterns and develop predictive models. 

## Problem Statement
How can we effectively predict the severity of traffic accidents when the severity levels are imbalanced? How can machine learning models be used to support better decision-making for road safety improvements?

## Dataset
Name: US Accidents March23 sampled 500k.csv

Source: Data from 49 U.S. states collected via multiple APIs (Departments of Transportation, law enforcement, traffic sensors).

## Features:

Accident ID, Location, Weather conditions (e.g., temperature, visibility), Time of day, Road conditions, Severity (1-4).

Severity Level: Ordinal scale — 1 (Minor) to 4 (Severe).

## Methodology
KDD Process:
Data Selection

Preprocessing

Transformation

Data Mining

Interpretation & Evaluation

Knowledge Presentation

Machine Learning Models:
Random Forest

Accuracy: 73%

F1 Score: Best performance on moderate accidents (Class 2)

XGBoost

Weighted F1 Score: 0.71

Utilized class weights to handle imbalance

LightGBM

Weighted F1 Score: 0.72

Excelled at Class 1 (moderate), struggled on Classes 0 & 3

All models handled imbalance using techniques such as SMOTE, class weighting, and custom evaluation metrics (like F1 score).

## Key Findings
Temperature, Wind Direction, and Sunrise/Sunset were strong indicators of accident severity.

Class imbalance significantly affected prediction accuracy, especially for severe accidents.

Using KDD and ensemble learning boosted performance and interpretability.

## Technologies Used
Python (Pandas, Scikit-learn, LightGBM, XGBoost)

SMOTE (for handling imbalance)

Jupyter Notebooks

GitLab (for collaboration)
