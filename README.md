# Fraud analytics
## 1. Data Description
`Dataset Name`: Property Valuation and Assessment Data Data Source: NYC Department of Finance

`Data Version`: 2010/11/17

`Number of Fields`: 32

`Number of Records`: 1070994

## 2. Data Analysis 

+ Exploratory Data Analysis

+ Data Cleaning: exclude properties own by the government and fill the missing values

+ Feature Creation: represent data with six features through PCA and normalized the result to prepare for the modeling. 

+ Dimensionality Reduction:

+ Fraud Model Algorithm: Establish two models for fraud score calculation

  1) Z score outliers by calculating each data point's Euclidean distance from the origin
  
  2) Autoencoder error which is the difference between the input and the output of the autoencoder vectors

+ Summarize Results : combine the two unscale scores to get the final rank of records
