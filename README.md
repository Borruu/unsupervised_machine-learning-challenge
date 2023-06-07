# Myopia Clusters
Use unsupervised machine learning to cluster patients in a Myopia study into distinct groups.

## Background

You are on the data science team of a medical research company that’s interested in finding better ways to predict myopia, or nearsightedness. Your team has tried — and failed — to improve their classification model when training on the whole dataset. However, they believe that there might be distinct groups of patients that would be better to analyse separately. So, your supervisor has provided you with raw data and asked you to explore this possibility by using unsupervised learning.

## Stages

* Part 1: Prepare the Data

* Part 2: Apply Dimensionality Reduction 

* Part 3: Perform a Cluster Analysis with K-means

* Part 4: Make a Recommendation 

### Part 1: Prepare the Data

1. Read `myopia.csv` into a Pandas DataFrame.

2. Remove the "MYOPIC" column from the dataset (this is the target column).

3. Standardise the dataset so that columns that contain larger values do not influence the outcome more than columns with smaller values.

### Part 2: Apply Dimensionality Reduction

1. Perform dimensionality reduction with PCA, preserving 90% of the explained variance. How did the number of the features change?

2. Further reduce the dataset dimensions with t-SNE and visually inspect the results.

3. Create a scatter plot of the t-SNE output. Are there distinct clusters?

### Part 3: Perform a Cluster Analysis with K-means

Create an elbow plot to identify the best number of clusters.

* Use a `for` loop to determine the inertia for each `k` between 1 through 10. 

* Determine where the elbow of the plot is, and at which value of `k` it appears.

![image](https://github.com/Borruu/unsupervised_machine-learning-challenge/assets/112932520/f9bd7d61-b19f-48dd-b736-4928f7203780)

### Part 4: Make a Recommendation
Recommendation of five clusters as per image above.

## References

Reduced dataset from *Orinda Longitudinal Study of Myopia* conducted by the US National Eye Institute https://clinicaltrials.gov/ct2/show/NCT00000169
