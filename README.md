# Vivek Bavda 

## Fair Housing: Predicting Sale Prices in Ames, IA .




## Problem Statement

As you are aware, Ms. Mayor of Ames, Iowa, there have been concerns about redlining, restrictive covenants, and discrimination by homesellers in our city toward traditionally disadvantaged groups in our country. Given the uproar and your desire to integrate the community, you've asked me to provide a gender and color neutral model of housing prices to determine if there has been a premium required for people of color on homes bought in Ames, Iowa.


Recommendation: Use the Ordinary Multivariate Linear Regression model to predict prices and determine if there is a premium for traditionally disadvantage. The model should be used to identify hosts of transactions and to deal with individual cases.


## Table of Contents in the Repository

A Jupyter Notebook [VivekBavdaProject2AmesHousingAnalysis.ipynb](VivekBavdaProject2AmesHousingAnalysis.ipynb) showing the detailed calculations and analysis.

The Data Dictionary can be accessed within this repository [*here*](datasets/AmesDataDictionary.pdf).

* **Ames Dataset Train** : Data set contains information from the Ames, Iowa Assessor’s Office used in computing assessed values for individual residential properties sold in Ames, IA from 2006 to 2010. This dataset has been divided into this train set and validation set by the Mayor for Bavda Consulting to use to create its model. T The data has 81 columns which include 22 nominal, 23 ordinal, 14 discrete, and 20 continuous variables (and 2 additional observation identifiers). 


* **AmesDatasetTest** Data set contains information from the Ames, Iowa Assessor’s Office used in computing assessed values for individual residential properties sold in Ames, IA from 2006 to 2010. This dataset has been divided into a train set (above) and a validation set. This validation set includes 80 of 81 columns which include 22 nominal, 23 ordinal, 14 discrete, and 19 continuous variables (and 2 additional observation identifiers). The missing column is Sale Price in this dataset. This data is to be filled by Bavda Consulting using the 81 columns. This ensures and checks that the model developed by Bavda Consulting accurately predicts the price.
    
    
* **AmesDatasetValidation**: Data set contains the predictions for the validation set. This dataset has been submitted to the Mayor alongside with this report and model.


Presentation slides can be found [*here*](BavdaHomePricesAmesSlides.pdf)

And this Readme.md



## Analysis and Conclusions


As the introduction explains, the Mayor has hired Bavda Consulting to develop a model that predicts prices on home sales in Ames, Iowa. The purpose of this model is to help the Mayor identify and root out discrimination in housing. The model will serve as a benchmark as a predictor based on non-discriminatory factors such as square feet, the age of the home, the amount of garage area, etc. This will demonstrate if traditionally disadvantaged communities are paying a premium on housing in Ames. 

The production model chosen was the Ridge Penalty Multivariate Linear Regression model. Given that the Mayor has deemed Root Mean Squared Error (RMSE) as her metric on her validation test, this model is the one that minimized RMSE on the validation check. However, my recommendation is to use the Ordinary Multivariate Linear Regression because this is a simpler model to explain to constituents.


The second recommendation would be to create an interactive version of the model on the city's website. Each buyer, advantaged or disadvantaged, could input the variables for the house they are seeking. The independent variables could be changed and played with. 


Each coefficient detailed in the modeling section could be assigned to its features.  Each one unit increase in the independent variable would suggest a coefficient increase in the sale price. This would guide the community in expectations of the appropriate price and alert buyers if they sense they are being made to pay a premium regardless of advantaged status.


Third, another more directly related to fair housing recommendedation is to send in two couples, one traditionally advantaged, and the other traditionally disadvantaged, to see if the prices agreed upon at the new home developer's office are similar. The model can serve as a benchmark to evaluate the discrepancy between the two prices to determine if a premium was required. The model also could be used to identify potential discrimination by entering in data from housing transactions to see if there is trend. The city would know where to use its limited resources.

Fourth, given that there can be many uses for a model that predicts sale prices and the city has limited resources, the Mayor may well license the model to real estate agencies to earn extra revenue to fund her fight for integration. This would be a win, win for both parties.


