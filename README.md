# Titanic – Machine Learning from Disaster
This README provides an overview of the Titanic Machine Learning project, including its motivation, installation requirements, data, implementation details, and initial results.

## Project Motivation

The sinking of the Titanic is one of the most infamous shipwrecks in history. On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew. While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others. In this challenge, we ask you to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (i.e., name, age, gender, socio-economic class, etc).

## Installation
- **Python V-3.**
- **Libraries:**
•	Scikit Learn.
•	Pandas.
•	Seaborn

## Data

For this project, there are two similar datasets that include passenger information like name, age, gender, socio-economic class, etc. One dataset is titled train.csv, and the other is titled test.csv. `train.csv` will contain the details of a subset of the passengers on board (891 to be exact) and importantly, will reveal whether they survived or not, also known as the “ground truth”. The `test.csv` dataset contains similar information but does not disclose the “ground truth” for each passenger. The aim is to predict these outcomes. Using the patterns to be found in the `train.csv` data, to predict whether the other 418 passengers on board (found in `test.csv`) survived.
You can check out the [Data](https://www.kaggle.com/competitions/titanic/data) tab on Kaggle to explore the datasets even further.

## Implementation

**The following actions were performed:**
- Data exploration
- Data visualization
- Feature selection
- Data engineering

**The following models were used:**
- RandomForestClassifier
- DecisionTreeClassifier
- LogisticRegression
- GradientBoostingClassifier
- KNeighborsClassifier

**Other functions used:**
- train_test_split
- confusion_matrix
- classification_report
- accuracy_score

## Results before GridSearch

- RandomForestClassifier – 83%
- DecisionTreeClassifier – 81%
- LogisticRegression – 82%
- GradientBoostingClassifier - 84%
- KNeighborsClassifier – 81%

Used GridSearchCV on `RandomForestClassifier` to search for the best parameters, which gave an 86% accuracy.
