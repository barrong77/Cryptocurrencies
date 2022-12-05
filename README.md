# Cryptocurrencies

The purpose of this project is to use unsupervised machine learning to analyze a database of cryptocurrencies.  In addition, create a report including the traded cryptocurrencies classified by group according to their features.
Ideally, this classification report could be used by an investment bank to propose a new cryptocurrency investment portfolio.

I used the following methods for the analysis:

preprocessing the database,
reducing the data dimension using Principal Component Analysis,
clustering cryptocurrencies using K-Means,
visualizing classification results with 2D and 3D scatter plots.

Data Preparation
Read crypto_data.csv into Pandas. 

Discarded all cryptocurrencies that are not being traded.

Removed all rows that have at least one null value.

Filtered for total coins mined should be greater than zero.

Converted the remaining features with text values, Algorithm and ProofType, into numerical data. To accomplish this task, used Pandas to create dummy variables.

Standardized the dataset so that columns that contain larger values do not unduly influence the outcome.

Dimensionality Reduction

For this project, preserved 90% of the explained variance in dimensionality reduction.


Cluster Analysis with k-Means
Created an elbow plot to identify the best number of clusters. Used a for-loop to determine the inertia for each k between 1 through 10. Determine, if possible, where the elbow of the plot is, and at which value of k it appears.

Results

Cryptocurrencies can be cluster into distinct groups.
