# Myopia Predictions using Unsupervised Machine Learning

## Background
I am on the data science team of a medical research company that’s interested in finding better ways to predict myopia, or nearsightedness. My team has tried—and failed—to improve their classification model when training on the whole dataset. However, they believe that there might be distinct groups of patients that would be better to analyze separately. So, my supervisor has asked you to explore this possibility by using unsupervised learning.

I have been provided with raw data, so I will first need to process it to fit the machine learning models. I will use several clustering algorithms to explore whether the patients can be placed into distinct groups. Then, I will create a visualization to share my findings with my team and other key stakeholders.

## Project Steps

## Part 1: Prepare the Data
    - Read the csv file into a Pandas DataFrame
    - Remove the "MYOPIC" column from the dataset
    - Standardize the dataset so that columns that contain larger values do not influence the outcome more than columns 
    with smaller values

## Part 2: Apply Dimensionality Reduction
    - Perform dimensionality reduction with PCA.
    - Preserve 90% of the explained variance in dimensionality reduction.
    - Further reduce the dataset dimensions wtih t-SNE and visually inspect the results. To do this, run the t-SNE on the 
    principal components, which is the output of the PCA transformation.
    - Create a scatter plot of the t-SNE output. Are there distinct clusters?

## Part 3: Perform a Cluster Analysis with K-means
Create an elbow plot to identify the best number of clusters.
    - Use a for loop to determine the inertia for each k between 1 through 10.
    - If possible, determine where the elbow of the plot is, and at which value of k it appears.

## Part 4: Recommendation
Can the patients be clustered? Based on the amount of data used, it would be difficult to cluster the patients. There were not distinct clusters shown when using the t-SNE model. The elbow curve chart was also not very distinct. It is more rounded curve than elbow shaped curve. This would not provide accurate enough information the supervisors are looking for.

## Tools used
Python, Pandas, Jupyter Notebook, Matplotlib, sklearn - PCA, TSNE, StandardScaler, KMeans
