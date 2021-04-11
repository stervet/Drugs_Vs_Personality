## Drug Risk and Personality Traits
Authors: 

## Overview
This project aims at examining the relationship between personality traits and drug consumption based on the [Drug consumption (quantified) Data Set](https://archive.ics.uci.edu/ml/datasets/Drug+consumption+%28quantified%29). The Dataset contains 35 variables of 1885 people.. First, the normalized data is coded into more apprehensible, numeric categories. Then further features are engineered to highlight deeper data structures. The engineered variables are: soft drug consumption, hard drug consumption, legal drug consumption, illegal drug consumption, synthetic and nonsynthetic drug consumption, recent consumtion, hard score and hardliners.

The hard score (hard_score) is build of the mean of neuroticism, extraversion, impulsiveness and sensation seeking. The hardliner variable, however, comprises only the 10% highest hard scores. Business Case

A drug prevention organization is interested in the use frequency of illegal drugs of hardliner personalities versus other people. Furthermore, they want to predict the use of illegal drugs.

The project was part of a data science bootcamp and should cover all stages of the data science cycle:

## Data Science Lifecycle
* 1 Business Understanding
* 2 Data Mining
* 3 Data Cleaning
* 4 Data Exploration
* 5 Feature Engineering
* 6 Predictive Modeling
* 7 Data Visualization
Python Modules used:
Pandas / NumPy / Matplotlib / Seaborn / Plotly / sklearn

## Used ML Models
Models were applied and compared for recall and accuracy scores

* XGBClassifier
* AdaBoost
* RandomForestClassifier
* Support Vector Machine
* DecisionTreeClassifier

## Summary
[x] Replaced the numeric data with the real names and deleted the 8 observation that had the fictional drug Semeron.
[x] Investigate the bias of our dataset and found out that we have very high level of education, very high rate of drug users and a abnormal difference of drug users between countries. This bias made us exclude the country and Ethnicity from our predictions.
[x] We separated our drugs to soft and hard according the the impact they have on health and the level of addiction they cause. We excluded smoking and alcohol, because almost everybody in our dataset drunk yesterday and the rate of smokers is incredibly high.
[x] our main definition of a drug user was a person the took drugs at least once in the last year. Later on we examined the the 'frequency' of using, ig. people that took drugs yesterday or people that never used.
[x] An exhaustive search with a pipeline was performed to select the most effective subset of input features. We then applied a grid search with our most promising features. We mainly took as the demographical personality features and made prediction of drug users. We can to the conclusion that high scores of Openness, Impulsiveness and sensession seeking behavior increase the risk for drug usage and that it is indeed possible to predict hard drug usage for "high scores"
[x] Reviewed the difference between gender and drug usage to find out that the rate of male drug users is significantly higher.

## Future Work
* Collect samples that allow the usage of the country feature and that represent the overall population of the countries
* Get time-related data to find out more about the relationship between drug usage and time-related factors
* Gather information about the effect of preventive actions regarding hard drug usage
* Use unsupervised learning algorithm to create clusters of different drugs and personality types
