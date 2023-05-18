# Surprise Housing - Advanced Regression Assignment

An advanced regression model to predict the actual value of the prospective properties.

---

## Table of Contents

- [General Info](#general-information)
- [Technologies Used](#technologies-used)
- [Conclusions](#conclusions)
- [Acknowledgements](#acknowledgements)

---

## General Information

Surprise Housing, a housing company located in the United States, has decided to enter the Australian market. The company employs data analytics to buy houses for less than their true value and resell them for more. The company has also gathered data from house sales in Australia for the same purpose. The company is looking at potential properties to purchase in order to enter the market. 

The goal is to create a regression model with regularisation in order to anticipate the actual worth of the potential properties and determine whether or not to invest in them. The organisation wants to discover which characteristics are significant in predicting property prices and how well those variables characterise house prices.

### Datasets

- [Data Set](https://ml-course3-upgrad.s3.amazonaws.com/Assignment_+Advanced+Regression/train.csv): This contains the sale of houses in Australia.
- [Data Definition](https://cdn.upgrad.com/UpGrad/temp/87f67e28-c47e-4725-ae3c-111142c7eaba/data_description.txt): The details of the various variables are given in this file.

---

## Conclusions

We have applied regularisation techniques and the below are the results.

|              | Linear        | Ridge         | Lasso         |
|--------------|---------------|---------------|---------------|
| R2 Score (Train)   | 9.367446e-01  | 0.885897      | 0.895105      |
| R2 Score (Test)    | -2.570889e+21 | 0.870696      | 0.864361      |
| RSS (Train)        | 7.975898e-01  | 1.438732      | 1.322625      |
| RSS (Test)         | 1.407576e+22  | 0.707947      | 0.742629      |
| MSE (Train)        | 7.858028e-04  | 0.001417      | 0.001303      |
| MSE (Test)         | 3.228384e+19  | 0.001624      | 0.001703      |
| RMSE (Train)       | 2.803217e-02  | 0.037649      | 0.036098      |
| RMSE (Test)        | 5.681887e+09  | 0.040296      | 0.041271      |

Using Ridge Regression, the following table shows the top 10 most important predictor variables,

| Feature                | Coefficient             |
|------------------------|-------------------------|
| GrLivArea              | 0.114259                |
| OverallQual            | 0.098885                |
| 2ndFlrSF               | 0.082416                |
| GarageCars             | 0.068762                |
| Condition2_PosN        | -0.066828               |
| Neighborhood_NoRidge   | 0.059324                |
| RoofMatl_WdShngl       | 0.053328                |
| TotalBsmtSF            | 0.043470                |
| Neighborhood_StoneBr   | 0.042255                |
| FullBath               | 0.040968                |

Using Lasso Regression, the following table shows the top 10 most important predictor variables,

| Feature                | Lasso                   |
|------------------------|-------------------------|
| Condition2_PosN        | -0.340414               |
| GrLivArea              | 0.339689                |
| OverallQual            | 0.123430                |
| RoofMatl_WdShngl       | 0.074416                |
| GarageCars             | 0.067505                |
| Neighborhood_NoRidge   | 0.058470                |
| Neighborhood_NridgHt   | 0.043794                |
| Neighborhood_StoneBr   | 0.042549                |
| 2ndFlrSF               | 0.040143                |
| RoofMatl_CompShg       | 0.033650                |

---

## Technologies Used

Python 3.10.11

| Library      | Version |
| ------------ | ------- |
| numpy        | 1.22.4  |
| pandas       | 1.5.3   |
| matplotlib   | 3.7.1   |
| seaborn      | 0.12.2  |
| sklearn      | 1.2.2   |

---

## Acknowledgements

- This assignment was done as a part of EPGP ML & AI, IIIT-B.
- [Data Set](https://ml-course3-upgrad.s3.amazonaws.com/Assignment_+Advanced+Regression/train.csv) and [Data Definition](https://cdn.upgrad.com/UpGrad/temp/87f67e28-c47e-4725-ae3c-111142c7eaba/data_description.txt) was provided by upGrad and IIIT-B.

---

Assignment done by: [Rahul Nanwani](https://github.com/rahul-nanwani)
