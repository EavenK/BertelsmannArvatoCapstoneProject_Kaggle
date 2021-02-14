# BertelsmannArvatoCapstoneProject_Kaggle

### Table of Contents

1. [Description](#description)
2. [Files](#files)
3. [Motivation](#motivation)
4. [Dependencies](#dependencies)
5. [Results](#results)
6. [Author](#author)
7. [Acknowledgement](#acknowledgement)


## Description <a name="description"></a>

This Capstone Project is part of the Data Science Nanodegree Program by Udacity in collaboration with [Bertelsmann Arvato]. The datasets consist of 366 features that described approximately 1 million individuals from the German population. 
The data were not 'clean' and required tremendous amount of data wrangling efforts. The aim of the project is to analyze demographics data for customers of a mail-order sales company in Germany, comparing it against demographics information for the general population. We will use unsupervised learning techniques to perform customer segmentation, identifying the parts of the population that best describe the core customer base of the company. Then apply what we have learned on a third dataset with demographics information for targets of a marketing campaign for the company, and train a model to predict which individuals are most likely to convert into becoming customers for the company.

## Files <a name="files"></a>

There are 4 datafiles associated with this project: 
* Udacity_AZDIAS_052018.csv - Demographics data for the general population of Germany (891211 x 366).
* Udacity_CUSTOMERS_052018.csv - Demographics data for customers of the German mail-order company (191652 x 369).
* Udacity_MAILOUT_052018_TRAIN.csv - Demographics data for individuals who were targets of a marketing campaign (42982 x 367).
* Udacity_MAILOUT_052018_TEST.csv - Demographics data for individuals who were targets of a marketing campaign (42833 x 366).

There are additional 2 metadata files provided and 1 manually created.
* DIAS Information Levels - Attributes 2017.xlsx - is a top-level list of attributes and descriptions, organized by informational category.
* DIAS Attributes - Values 2017.xlsx - is a detailed mapping of data values for each feature in alphabetical order.
* feat_info.csv - is a feature summary file manually created using the above 2 files together with a previous subset feature_info.csv from 1st semester mapping all the attributes with information level, type & missing_or_unknown information to assist in our analysis.

These datasets are not available here due to confidentiality.

## Motivation <a name="motivation"></a>
The reason I choose this Capstone project provided by Bertelsmann Arvato is because
 - I can used unsupervised machine learning and supervised machine learning techniques in 1 same project.
 - This project provide me an opportunity to parcipate in Kaggle competition. 

<a name="dependencies"></a>
### Dependencies
* Python 3.5+ 
* Machine Learning Libraries: NumPy, SciPy, Pandas, Scikit-Learn, xgBoost, LightGBM, CatBoost
* Model Loading and Saving: Pickle

 - pip install jupyter-tensorboard==0.1.10
 - pip install scikit-learn==0.22.2
 - pip install lightgbm==3.1.1
 - pip install xgboost==1.0.2
 - pip3 install catboost==0.23.2
 - pip install "scikit_optimize==0.7.4" 

## Results<a name="results"></a>

* Part 1 Data Preprocessing
> It was necessary to apply CRISP-DM (Cross-Industry Standard Process for Data Mining) to the project. Data Understanding, Data Preparation, Modelling and Evaluation had to be developed from scratch.
* Part 2 Customer Segmentation Report
 > The project used unsupervised learning methods to analyze attributes of established customers and the general population in order to create customer segments. Unsupervised learning techniques namely PCA and Clustering with KMeans were applied to distinguish groups of individuals that best describe the core customer base of the mail-order company.
* Part 3 Supervised Learning Model
> Used the previous analysis to build a machine learning model that predicts whether or not each individual will respond to the campaign. The base performance of various classifiers were determined. CatBoost was being picked and with the help of BayesSearchCV, the model was further optimized and tuned (using stratified K-Fold cross-validation) and its performance was evaluated via ROC AUC. A short analysis of the features importance is being performed. The best model is then used to predict the testing dataset where individuals of a marketing campaign are more likely being convert into company's customer.
* Part 4 Kaggle Competition
> Once chosen a model, use it to make predictions on the campaign data as part of a Kaggle Competition. Result was submitted to obtain a kaggle score which is roc_auc score on the testing data. Through Kaggle score, position of the participant in the leaderboard was determined.

For the full analysis, please visit my blog post available here [Create a Customer Segmentation Report for Arvato Financial Services](https://eavenkhaw.medium.com/create-a-customer-segmentation-report-for-arvato-financial-services-129f5ceaf14d).


## Author<a name="authors"></a>

* [Eaven Khaw](https://github.com/EavenK)


## Acknowledgements<a name="acknowledgement"></a>

* [Udacity](https://www.udacity.com/) as hosts of the Data Science Nanodegree Program
* [Arvato](https://www.arvato.us/), subsidiary of [Bertelsmann](https://www.bertelsmann.com/#st-1) for providing the datasets 
