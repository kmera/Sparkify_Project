1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

The libaries needed to run the code, using Python version 3.* are:

* Pandas
* NumPy
* Matplotlib
* Seaborn
* PySpark SQL
* PySpark ML
* scikit-learn

## Project Motivation<a name="motivation"></a>

Using Sparkify tiny subset (128MB) of the full dataset available (12GB), the goal is to predict customer churn. Sparkify is a music stream app which has free users (includes advertising) and paid users who have to paid a monthly rate. Besides, users can downgrade, upgrade or cancel the service anytime.  

There are many reasons a user would churn such as: infeffective recommendations which are not aligned with the genres user preferences, songs they want to listen but are not available in sparkify, complex or useless app UI/UX, cost of the service, and so on, so the feature engineering will support us to consider some of this reasons. I have considered this problem as a binary classification (churn / not churn), so I will use Logistic and Random Forest models to fit the data and predict churn.

## File Descriptions <a name="files"></a>

There is one notebook that was developed according to the following steps:

* Load and Clean Dataset, checking for invalid or missing data - for example, records without userids or sessionids.
* EDA, create a column Churn to use as the label for your model, and perform some exploratory data analysis to observe the behavior for users who stayed vs users who churned
* Feature Engineering, build out the features you find promising to train your model on
* Modeling, split the full dataset into train, test, and validation sets. Test out several of the machine learning methods, and evaluate the accuracy of the various models, tuning parameters as necessary.

## Results<a name="results"></a>

As was mentioned before, for this project were considerd two ML models: Logistic Regression and Random Forest.
* Logistic Regression:
Accuracy: 77.14%
'f1_score': 0.42857142857142855, 'precision': 0.375, 'recall': 0.5

* Random Forest:
Accuracy: 77.14%
'f1_score': 0.42857142857142855, 'precision': 0.375, 'recall': 0.5

Taking account the results of both Logistic Regression and Random Forest, it seems that Random Forest is the best model for this project. 

Moreover, the main findings of the code can be found at the medium post [Predicting Churn Rate for 'Sparkify' stream music app](https://medium.com/@klever.mera/thinking-to-travel-to-boston-after-the-lockdown-f84a99ec728e).

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Must give credit to [Udacity](https://cn.udacity.com/) 

