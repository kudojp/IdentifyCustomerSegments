# IdentifyCustomerSegments

This is my 3rd project in Udacity Data Scientist Nanodegree Program. I used unsupervised learning and PCA to identify the cluster of customers of a mail-order sales company.


## Project Overview
In this project, these 2 datasets are provided. 

```
1. Demographic information about the people of Germany
2. The same information for customers of a mail-order sales company
```

I’ll look at relationships between demographics features, organize the population into clusters, and see how prevalent customers are in each of the segments obtained.

## Dataset Details

* Udacity_AZDIAS_Subset.csv: Demographic data for the general population of Germany; 891211 persons (rows) x 85 features (columns).
* Udacity_CUSTOMERS_Subset.csv: Demographic data for customers of a mail-order company; 191652 persons (rows) x 85 features (columns).
* Data_Dictionary.md: Information file about the features in the provided datasets.
* AZDIAS_Feature_Summary.csv: Summary of feature attributes for demographic data.


## Project Details

#### Step 1: Preprocessing

I will create a cleaning procedure first to the general demographic data, then later to the customers data.

* How are missing or unknown values encoded in the data? 
* Are there certain features (columns) that should be removed from the analysis because of missing data? 
* Are there certain data points (rows) that should be treated separately from the rest?
* Consider the level of measurement for each feature in the dataset (e.g. categorical, ordinal, numeric). 
* What assumptions must be made in order to use each feature in the final analysis? 
* Are there features that need to be re-encoded before they can be used? 
* Are there additional features that can be dropped at this stage?

#### Step 2: Feature Transformation

Now that my data is clean, I will use dimensionality reduction techniques to identify relationships between variables in the dataset, resulting in the creation of a new set of variables that account for those correlations. 

* The first technique that you should perform on your data is feature scaling. What might happen if we don’t perform feature scaling before applying later techniques you’ll be using?

* Once you’ve scaled your features, you can then apply PCA to find the vectors of maximal variability. How much variability in the data does each principal component capture? Can you interpret associations between original features in your dataset based on the weights given on the strongest components? How many components will you keep as part of the dimensionality reduction process?


#### Step 3: Clustering
Finally, I will apply clustering techniques to identify groups in the general demographic data. I will then apply the same clustering model to the customers dataset to see how market segments differ between the general population and the mail-order sales company.

* Use the k-means method to cluster the demographic data into groups. How should you make a decision on how many clusters to use?
* Apply the techniques and models that you fit on the demographic data to the customers data: data cleaning, feature scaling, PCA, and k-means clustering. Compare the distribution of people by cluster for the customer data to that of the general population. Can you say anything about which types of people are likely consumers for the mail-order sales company?
