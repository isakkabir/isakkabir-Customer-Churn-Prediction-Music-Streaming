# isakkabir-Customer-Churn-Prediction-Music-Streaming 

### 1. Project Overview

We want to identify the users that could potentially cancel their account and leave the service. Our goal in this project was to help a fictional business (similar to Spotify and Pandora) by building and training a binary classifier that is able to accurately identify users who cancelled the music streaming service, based on the patterns obtained from their past activity and interaction with the service.
**Define churn variable** : 1 - users who cancelled their subscription within the observation period, and 0 - users who kept the service throughout


### 2. Model Development Approach

The model development process consists of three main steps that can be summarised as follows.

#### Data Understanding

* Generate population statistics and understand different variables, their type, range/categories, distribution, etc. Understanding the relationships between different columns.
* Identifying missing values and potential duplicates

#### Feature Engineering and Exploratory Data Analysis

* Pre-processing (cleaning & transformation) the original data-set (one row per user log) to a data-set with user-level information or statistics (one row per user).
* Use Feature engineering to identify churned users, e.g. aggregated statistic per unit of time, number of plan changes, songs played vs. total activity ratio, thumbs up vs. thumbs down ratio, activity trend, etc.
* Exploratory analysis, comparing the engineered statistics for users who stayed vs users who churned and the correlation between engineered features
* Standardisation of the numerical features and feature assembly

#### Modelling and Evaluation

* Defining pipelines for binary classifiers (logistic regression, random forest classifier or gradient boosting classifier) using Grid-search, splitting the data-set into training and test set. 
* Evaluate model performance using F1 score and extracting feature importances
* Retraining the best-performing models on the full training set
