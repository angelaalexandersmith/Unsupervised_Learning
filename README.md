# Unsupervised_Learning

Instructions
This activity is broken down into four parts:

Part 1: Prepare the Data.

Part 2: Apply Dimensionality Reduction.

Part 3: Perform a Cluster Analysis with K-means.

Part 4: Make a Recommendation.

Part 1: Prepare the Data
Read myopia.csv into a Pandas DataFrame.
![image](https://user-images.githubusercontent.com/108265105/202068820-bc85bfed-1aa6-42d3-a0d2-3424022c475d.png)


Remove the "MYOPIC" column from the dataset.

Note: The target column is needed for supervised machine learning, but it will make an unsupervised model biased. After all, the target column is effectively providing clusters already!
Standardise your dataset so that columns that contain larger values do not influence the outcome more than columns with smaller values.

Part 2: Apply Dimensionality Reduction
Perform dimensionality reduction with PCA. How did the number of the features change?
Hint: Rather than specify the number of principal components when you instantiate the PCA model, state the desired explained variance. For example, say that a dataset has 100 features. Using PCA(n_components=0.99) creates a model that will preserve approximately 99% of the explained variance, whether that means reducing the dataset to 80 principal components or 3. For this assignment, preserve 90% of the explained variance in dimensionality reduction.
Further reduce the dataset dimensions with t-SNE and visually inspect the results. To do this, run t-SNE on the principal components, which is the output of the PCA transformation.

Create a scatter plot of the t-SNE output. 
![image](https://user-images.githubusercontent.com/108265105/202068960-807113b4-f9df-46f6-96cb-e42ac740ae43.png)


Part 3: Perform a Cluster Analysis with K-means
Create an elbow plot to identify the best number of clusters. Make sure to do the following:

Use a for loop to determine the inertia for each k between 1 through 10.

![image](https://user-images.githubusercontent.com/108265105/202070050-f09a4e0f-3444-4d4a-94f2-1cdc6352ec65.png)


Part 4: Make a Recommendation
Based on your findings, write up a brief (one or two sentences) recommendation for your supervisor in your Jupyter Notebook. Can the patients be clustered? If so, into how many clusters?

![image](https://user-images.githubusercontent.com/108265105/202070184-f26bd095-8a2d-4a6a-b2ad-bc987f67b226.png)
