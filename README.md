# Cryptocurrencies
## Project Overview
With the help of unsupervised machine learning methodology to investigate a dataset of different cryptocurrencies and develop trends to deliver an investment portfolio to Martha's firm, Accountability Accounting. During this process, we learned how to cluster, transform and process data by reducing data dimensions and principal companents using PCA

## Resources
Data Sources provided to analyze and minipulate included:

crypto_data.csv
Software utilized for this study included:

Python 3.8.2
Pandas
Personal GitHub account

## Analysis/Workflow/Results

 Specifically for this deliverable we did the following:

1. Read in the crypto_data.csv to the Pandas DataFrame named crypto_df.
2. Keep all the cryptocurrencies that are being traded.
3. Drop the IsTrading column.
4. Remove rows that have at least one null value.
5. Filter the drop_CoinName DataFrame so it only has rows where coins have been mined.
6. Create a new DataFrame that holds only the cryptocurrency names, and use the drop_CoinName DataFrame index as the index for this new DataFrame.
7.Remove the CoinName column from the drop_CoinName DataFrame since it's not going to be used on the clustering algorithm (see below).
![](dropcoinname.png?raw=true)
8. Use the get_dummies() method to create variables for the two text features, Algorithm and ProofType, and store the resulting data in a new DataFrame named X.
9. Use the StandardScaler fit_transform() function to standardize the features from the X DataFrame.
![](standardscaler.png?raw=true)

# Deliverable 2: Reducing Data Dimensions Using PCA
Specifically for this deliverable we did the following:

1. Continue using the crypto_clustering.ipynb file from Deliverable 1 where you’ve already performed the preprocessing steps.
2.Using the information we’ve provided, apply PCA to reduce the dimensions to three principal components.
3. Create a new DataFrame named pcs_df that includes the following columns, PC 1, PC 2, and PC 3, and uses the index of the crypto_df DataFrame as the index (see below).
![](threePCA.png?raw=true)
