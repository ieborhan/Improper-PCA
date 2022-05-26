# Improper PCA

PCA is an unsupervised dimensionality reduction technique that computes the eigenvalues of the covariance matrix (d*d matrix, d is the dimension that is 784 here). These eigenvalues (d=784) are the variance of the data. All of the 784 dimensions have 100% variance. It is crucial to preserve most of the variance while reducing the dimensions. 
 
We can set the number of the components (for example n_components=200). However, we do not know the explained variance of the data if we choose the principal component numbers manually. Do not choose the number of components, you may determine the explained variance ratio (for example 0.95 or 0.99 whatever you want). The best way is graphing the explained variance and principal components to decide the optimum number of components (Let's call it as Dimension-Variance tradeoff).

In this scenario, we are going to misapply PCA (We will fit the test data while applying PCA).
We know that it will cause the data leakage, however we do not have a chance to see the data leakage concretely. 

Could there be any other issue besides data leakage? A visible issue. Let's check it out and feel it.
