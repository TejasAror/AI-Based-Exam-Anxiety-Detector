# Student-Stress-Level-Prediction

## Problem definition 
In this project, we have developed a stress level prediction system from student data using supervised learning techniques. First, we analyzed student data to extract useful features. For example, we investigate how stress level of a student is impacted by social or environmental factors and which factor has the greater impact. Then we trained different ML models to predict the stress level accurately. Finally, We used validation matrices to compare and tune our model.  

## Brief description of the data 

URL: https://www.kaggle.com/datasets/rxnach/student-stress-factors-a-comprehensive-analysis 

The dataset we used contains 21 features related to stress on a student. The features were chosen using 5 main categories: Psychological, Physiological, Social, Environmental, and Academic factors. Some of the factors are anxiety level, sleep quality, living conditions, academic performance, and peer pressure. Features including anxiety level, depression, and self-esteem are on a scale from 0 to 30 while most other factors are on a scale from 0 to 5. Data has been collected from 1,100 students. 

## Project Outcome
Initially, there were three stress levels: 0, 1, 2. We merged Labels 1 and 2 as 1 and got two stress levels: 0 (No), 1(Yes)
After processing, The problem becomes a binary classification problem. We applied KNN, DT, and Random Forest classification to our dataset. We tuned the models with different sets of hyper-parameters to get the optimized model. Sklearn's GridSearchCV is used with 5-fold cross validation to construct parameter grids for hyperparameter tuning. Overall, the KNN and random forest tree performed best. In future, implementing neural network-based classification can improve performance and scalability.
