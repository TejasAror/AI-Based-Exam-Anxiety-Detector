# AI-Based Exam Anxiety Detector

An intelligent machine learning system designed to predict exam anxiety levels in students using psychological, academic, and environmental factors.

The project analyzes behavioral and lifestyle data to classify whether a student is likely to experience exam-related anxiety, enabling early identification and support for students facing stress.

## OVERVIEW

The AI-Based Exam Anxiety Detector uses supervised machine learning algorithms to analyze student data and predict anxiety levels before examinations.

Traditional stress detection relies on manual surveys and observations. This system instead leverages data-driven prediction models to detect patterns in student behavior and environmental conditions.

By analyzing multiple stress-related indicators, the system can automatically classify student anxiety levels and help educators identify students who may require support.

## DATASET

Dataset Source:
                
                https://www.kaggle.com/datasets/rxnach/student-stress-factors-a-comprehensive-analysis

Dataset Details

Total records: 1100 students

Total features: 21

Categories of features:

Psychological Factors

Physiological Factors

Social Factors

Environmental Factors

Academic Factors

Example Features

anxiety_level

self_esteem

depression

sleep_quality

headache

study_load

peer_pressure

academic_performance

social_support

living_conditions

Some psychological metrics (anxiety, depression, self-esteem) are scaled 0–30, while most other features are scaled 0–5.


## MACHINE LEARNING MODELS USED

Three supervised machine learning algorithms were implemented and compared:

1. K-Nearest Neighbors (KNN)

Identifies the class of a data point based on the majority class of its nearest neighbors.

2. Decision Tree

Builds a hierarchical tree structure using feature splits to classify student anxiety levels.

3. Random Forest

An ensemble learning method that combines multiple decision trees to improve prediction accuracy.


## MODEL OPTIMIZATION

Hyperparameter tuning was performed using:

GridSearchCV with 5-fold cross validation.

This approach tests multiple parameter combinations and selects the configuration that produces the best model performance.

## MODEL EVALUATION

The models were evaluated using the following metrics:

ROC Curve

Measures the model's ability to distinguish between anxiety classes.

Confusion Matrix

Shows the number of correct and incorrect predictions.

Precision–Recall Curve

Evaluates how well the model identifies true anxiety cases.

## PROJECT WORKFLOW

              Student Stress Dataset
                       ↓
           Data Cleaning & Preprocessing
                       ↓
               Feature Selection
                       ↓
             Train/Test Split (80/20)
                       ↓
                 Feature Scaling
                       ↓
              Machine Learning Models
          (KNN, Decision Tree, Random Forest)
                       ↓
            Hyperparameter Tuning
              (GridSearchCV)
                       ↓
               Model Evaluation
           ROC Curve • Confusion Matrix • Precision-Recall
                       ↓
            Exam Anxiety Prediction

## Project Outcome
Initially, there were three stress levels: 0, 1, 2. We merged Labels 1 and 2 as 1 and got two stress levels: 0 (No), 1(Yes)
After processing, The problem becomes a binary classification problem. We applied KNN, DT, and Random Forest classification to our dataset. We tuned the models with different sets of hyper-parameters to get the optimized model. Sklearn's GridSearchCV is used with 5-fold cross validation to construct parameter grids for hyperparameter tuning. Overall, the KNN and random forest tree performed best. In future, implementing neural network-based classification can improve performance and scalability.
