# Cryptocurrencies

# Bootcamp: UCB-VIRT-DATA-PT-03-2020-U-B-TTH

### Bootcamp Challenge #18 - 7/12/2020
Bootcamp Challenge 18: Module Unsupervised Machine Learning - Cryptocurrencies

### Links Used
- [crypto_data](https://courses.bootcampspot.com/courses/140/files/38734/download?download_frd=1)

### Challenge Description
**Objectives**
The goals for this challenge are for you to:
- Prepare the data for dimensions reduction with PCA and clustering using K-means.
- Reduce data dimensions using PCA algorithms from sklearn.
- Predict clusters using cryptocurrencies data using the K-means algorithm form sklearn.
- Create some plots and data tables to present your results.

## Technologies Used
- Jupyter Notebook
- Python, Pandas, PCA, plotly express, scatter plots, 3D scatter plots, hvplot.table, hvplot.scatter
- sklearn, K-means algorithm, clustering, scatter 
- GIT

## Methodology, Summary, Purpose 
After reading the cyrpto data from the CSV into a DataFrame, the challenge had us do various preprocessing steps on the data. I used the various Pandas dataframes functions to perform those functions. I then used pandas to create dummies and then used standard scaler from sklearn to perform a fit_transform on the X dataframe.  I then created a new PCA model with 3 components. I used the previous crypto_scaled_df to then fit_transform stored as crypto_pca which was ultimately used to create pcs_df.

I then effectively looped to create various KMeans models with different clusters. I then fit the data with the same dataframe, and plotted the respective inertia to demonstrate the elbow curve. From here we could observe k = 4 as the optimal value. I then run the model with k=4, add the CoinName and Class columns as requested, finally plotted them. Plots used: px.scatter_3d, hvplot.table, hvplot.scatter.
