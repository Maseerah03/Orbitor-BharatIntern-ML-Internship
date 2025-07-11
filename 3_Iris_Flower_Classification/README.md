# Iris Flower Classification using K-Means Clustering

## Project Overview

This project applies unsupervised learning (K-Means Clustering) to classify the famous Iris dataset into different flower species based on their sepal and petal features. The objective was to group the data without using the actual species labels and then evaluate how well clustering matched the original species.

## Dataset

The [Iris dataset](https://en.wikipedia.org/wiki/Iris_flower_data_set) is loaded directly using Seaborn's built-in dataset. It contains 150 samples with 4 numerical features:
- Sepal length
- Sepal width
- Petal length
- Petal width

## Key Tasks Performed

- Data exploration and preprocessing
- Visual analysis using 2D and 3D scatter plots
- Implementation of the Elbow Method to determine the optimal number of clusters
- Clustering using the KMeans algorithm
- Comparison of predicted clusters with actual species using a confusion matrix

## Tools and Libraries Used

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- scikit-learn

## Results

- KMeans clustering correctly identified the natural groupings in the data.
- The confusion matrix was used to measure how well the clusters matched the true species labels, showing a reasonably good alignment.

## Conclusion

This project demonstrates how unsupervised learning can discover patterns in data without relying on labeled outcomes. Though clustering doesn't always align perfectly with actual labels, it is a powerful tool for exploratory data analysis.
