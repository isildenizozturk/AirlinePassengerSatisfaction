# Airline Passenger Satisfaction Prediction with Classification

## Introuduction

The airline industry assembles an important part of the wider travel industry, by providing customers with the ability to purchase seats on flights and travel to different parts of the world.  There are a lot of airline companies that customers can choose and because of that, the airline companies face challenges as it's hard to differentiate. In order to be successful in the industry, companies need to understand customers’ exceptions. Satisfaction can change from person to person. But generally, if the product has at least met the needs of the consumer then it is said to be customer satisfaction. We attempt to understand the reasons for customer experience being satisfied or not by using a dataset from kaggle. As part of the analysis, we will be able to understand several factors which improve customer satisfaction level by using the obtained Airplane Passenger Satisfaction dataset.

## Problem 

Nowadays, people can easily access all kinds of information they are looking for over the internet and easily share their experiences, especially through social media. So, the most important factor in the success of companies is customer satisfaction. The companies in the industry are identifying a customer’s satisfaction through a rating card.

The research is about classifying if the customer is satisfied or not by finding out the factors related to high satisfaction of customers with airline services and developing a better understanding of the main quality factors that affect customer satisfaction, through examination of customers’ feedback and ratings.

## Dataset

We obtained our dataset which is Airline Passenger Satisfaction from Kaggle. By using this dataset we will try understand the factors to satisfy the customer. The dataset contains a total of 129.880 observations and 25 attributes. 

Dataset Source: https://www.kaggle.com/teejmahal20/airline-passenger-satisfaction. 

## Data Preparation

We import the dataset into Python and observe the structure of the data. The Satisfaction level, which is our dependent variable, is represented as a factor (“Satisfied” and “Neutral or Dissatisfied”). This dataset contains an airline passenger satisfaction survey. For preparing the data, first, we drop the unnecessary columns which we do not need in our analysis and model. Some data mining algorithms cannot handle categorical variables and after finding categorical values, we convert them into numerical values. The missing values can be a big problem because algorithms need to process the values. Therefore, we check our dataset for any possible NA values, which must be dealt with before we proceed with building the model.

## Data Exploratory Analysis

We did data analysis by looking at the distribution of different independent variables. Our
key variables are age, gender, customer type, type of travel, class, satisfaction, etc and other
various attributes that customers have given their ratings on such as seat comfort, inflight
entertainment, etc. which they will also decide on whether or not customers are satisfied overall
and at the end it gives us, the dependent variable called satisfaction. To verify and visualize the
relationship between the satisfaction variable and other key independent variables, we made
statistical research and a series of plots.


## Data Mining Algoritms

In this study, we trained 7 different classification models even though there are a lot of
classification algorithms.  In addition, we ran all of the 7 classifiers with their default parameters.

Random Forest (RF)
Logistic Regression (LR)
Decision Tree (CART)
K-Nearest Neighbor (KNN)
Gaussian Naïve
Bayes (GNB)
Gradient Boosting (GBM)  
LightGBM (LGBM).

## Experiments and Results

We created five different experiment datasets so that we can test classification models that we
choose on these datasets to get a better understanding of satisfaction. It helped us to see better the
attributes that have the most or no effect on passenger satisfaction. In order to select the
attributes for experiment datasets, we used the values on the table below which is for partitioning
the independent and dependent data. We choose gender, online boarding and inflight wifi service for using
in the dataset. We used Precision, Recall, F-Score, ROC Area and Accuracy metrics in order to measure
algorithms’ performance and compare them to each other for finding the best algorithm. If these
metric values are higher on one of the algorithms we selected, then we can say that it has the
higher performance and it is better for our study which is prediction of passenger satisfaction.


## Conclusion

In this study we used Airline Passenger Satisfaction dataset and classification models to help to
get better satisfaction from passengers, and evaluate a solution for their dissatisfaction. After
cleaning the dataset and doing some preprocessing steps like dropping unnecessary columns, we
make it ready for classification algorithms use.

We select 7 models for predicting satisfaction and choose the best one according to some metric scores. Also we compared them with some of the models who had good scores and performed very well and one of them failed badly compared to the other 6. However, RF and LGBM performed the highest scores on all of the cases, datasets and of course one of them has to be the best one which is the LGBM, it had a scores slightly higher than RF in some datasets, and happened to be the best model for airline passenger satisfaction prediction.

