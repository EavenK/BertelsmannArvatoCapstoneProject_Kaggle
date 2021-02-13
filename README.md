# BertelsmannArvatoCapstoneProject_Kaggle

### Table of Contents

1. [Description](#description)
2. [Dependencies](#dependencies)
3. [Author](#author)
4. [Results](#results)
5. [Acknowledgement](#acknowledgement)


## Description <a name="description"></a>

This Capstone Project is part of the Data Science Nanodegree Program by Udacity in collaboration with [Bertelsmann Arvato]. The datasets consist of 366 features that described approximately 1 million individuals from the German population. These datasets are not available here due to confidentiality:
* Udacity_AZDIAS_052018.csv 
* Udacity_CUSTOMERS_052018.csv
* Udacity_MAILOUT_052018_TRAIN.csv
* Udacity_MAILOUT_052018_TEST.csv

The data were not 'clean' and required tremendous amount of data wrangling efforts. The aim of the project is to analyze demographics data for customers of a mail-order sales company in Germany, comparing it against demographics information for the general population. We will use unsupervised learning techniques to perform customer segmentation, identifying the parts of the population that best describe the core customer base of the company. Then apply what we have learned on a third dataset with demographics information for targets of a marketing campaign for the company, and train a model to predict which individuals are most likely to convert into becoming customers for the company.


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

* Part 1 Customer Segmentation Report
 > Begin the project by using unsupervised learning methods to analyze attributes of established customers and the general population in order to create customer segments.
* Part 2 Supervised Learning Model
> Use the previous analysis to build a machine learning model that predicts whether or not each individual will respond to the campaign. 
* Part 3 Kaggle Competition
> Once chosen a model, use it to make predictions on the campaign data as part of a Kaggle Competition. Rank the individuals by how likely they are to convert to being a customer

There is a blog post available [here](https://medium.com/@eavenkhaw/write-a-data-science-blog-post-b574e36b5c19).


## Author<a name="authors"></a>

* [Eaven Khaw](https://github.com/EavenK)


## Acknowledgements<a name="acknowledgement"></a>

* [Udacity](https://www.udacity.com/) as hosts of the Data Science Nanodegree Program
* [Arvato](https://www.arvato.us/) , subsidiary of [Bertelsmann](https://www.bertelsmann.com/#st-1) for providing the datasets 
