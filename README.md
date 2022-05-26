# improper-pca

PCA is an unsupervised dimensionality reduction technique. PCA computes the eigenvalues of the covariance matrix (d*d matrix, d is the dimension, d is 784 here). These eigenvalues (784) are the variance of the data. All of the 784 dimensions have 100% variance. It is crucial to preserve most of the variance while reducing the dimension. 
 
We can set the number of the components (for example n_components=200) in Scikit-learn (2). However, we do not know the explained variance of the data if we choose the principal component numbers manually. Do not choose the number of components, instead determine the explained variance ratio (for example 0.95 or 0.99 whatever you want). You may graph the explained variance and principal components to decide the optimum number of components (Dimension-Variance tradeoff).
