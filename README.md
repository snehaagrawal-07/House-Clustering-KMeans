# House Clustering using K-Means

## Objective
Group California houses into clusters based on location, income, and price.

## Dataset
California Housing Prices (Kaggle) - housing.csv

## Methodology
1. Data cleaning (missing values, duplicates)
2. Feature scaling (StandardScaler)
3. Elbow method + Silhouette score to choose K (K=3)
4. K-Means clustering
5. Visualization and cluster analysis

## How to Run
pip install -r requirements.txt
jupyter notebook House_Clustering_KMeans.ipynb

## Results
We used K-Means with K = 3 and got three clusters. Mostly they are formed on the basis of location and size of the area, not just price.

Cluster 0 (Southern California, around Los Angeles):
Average house value is about $214,159 and median income is 3.87. Houses are around 30 years old on average. This is a medium range cluster.

Cluster 1 (Northern California, Bay Area side):
This one has the lowest average house value (about $193,450) and the lowest income (3.73). Houses are also around 30 years old.

Cluster 2 (Central California):
This cluster has the highest house value (about $229,325) and the highest income (4.65). The houses here are newer (about 15 years old) and the areas are much bigger, with more rooms and population than other clusters.

What we found:
- Areas with higher income generally have higher house prices.
- The difference in price between clusters is not very big, so clusters are mainly based on location and area size.
- Silhouette score is 0.296, so the clusters are separated only moderately and some overlap is there.
- The dataset is from the 1990 census, so the prices are old and not like today's market.

## Team
Sneha Deepak Agrawal