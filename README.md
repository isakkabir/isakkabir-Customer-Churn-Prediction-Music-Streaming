# isakkabir-Customer-Churn-Prediction-Music-Streaming 

### 2. Model Development Approach

The model development process consists of three main steps that can be summarised as follows.

#### Data Understanding

* Generate population statistics and understand different variables, their type, range/categories, distribution, etc. Understanding the relationships between different columns.
* Identifying missing values and potential duplicates

Feature Engineering and Exploratory Data Analysis

* Pre-processing (cleaning & transformation) the original data-set (one row per user log) to a data-set with user-level information or statistics (one row per user).
* Use Feature engineering to identify churned users, e.g. aggregated statistic per unit of time, number of plan changes, songs played vs. total activity ratio, thumbs up vs. thumbs down ratio, activity trend, etc.
* Exploratory analysis, comparing the engineered statistics for users who stayed vs users who churned and the correlation between engineered features
* Standardisation of the numerical features and feature assembly

Modelling and Evaluation

* Defining pipelines for binary classifiers (logistic regression, random forest classifier or gradient boosting classifier) using Grid-search, splitting the data-set into training and test set. 
* Evaluate model performance using F1 score and extracting feature importances
* Retraining the best-performing models on the full training set
