# Dimensionality-Reduction
This is an implementation of 3 dimensionality reduction techniques - PCA, SVD, and tSNE for visualization of high dimensional data in 2D and 3D.  

In this notebook, I have used 3 methods of Dimensionality Reduction:

- Principal Component Analysis
- Singular Value Decomposition
- t-distributed Stochastic Neighbor Embedding

I have used these techniques on two datasets:

- The Digits Dataset from sklearn
- MNIST Dataset - The "Hello World" of Computer Vision

t-SNE is an O(n^2) algorithm and the MNIST dataset was too large for it. I randomly sampled 10000 images from MNIST for visualization both in 2D and 3D.

## Performance Table
| Algorithm         | Digits Dataset         | MNIST Dataset (10000 images)  |
| ------------- |:--------------|:-----|
| PCA - 2 Components | 21.7 ms | 428 ms |
| SVD - 2 Components | 30.2 ms | 392 ms |
| tSNE - 2 Components | 10.4 s | 4 min 8 s |
| PCA - 3 Components | 29.9 ms | 457 ms |
| SVD - 3 Components | 26.8 ms | 336 ms |
| tSNE - 3 Components | 43.4 s | 12 min 35 s |


# Visualizations

## The Digits Dataset

### In 2 Dimensions
![Digits-PCA-2-Components](https://github.com/KhyatiMahendru/Dimensionality-Reduction/blob/master/Visualizations/digits-pca-2.png)
![Digits-SVD-2-Components](https://github.com/KhyatiMahendru/Dimensionality-Reduction/blob/master/Visualizations/digits-svd-2.png)
![Digits-TSNE-2-Components](https://github.com/KhyatiMahendru/Dimensionality-Reduction/blob/master/Visualizations/digits-tsne-2.png)

### In 3 Dimensions
![Digits-PCA-3-Components](https://github.com/KhyatiMahendru/Dimensionality-Reduction/blob/master/Visualizations/digits-pca-3.png)
![Digits-SVD-3-Components](https://github.com/KhyatiMahendru/Dimensionality-Reduction/blob/master/Visualizations/digits-svd-3.png)
![Digits-TSNE-3-Components](https://github.com/KhyatiMahendru/Dimensionality-Reduction/blob/master/Visualizations/digits-tsne-3.png)


## The MNIST Dataset (10000 images)

### In 2 Dimensions
![MNIST-PCA-2-Components](https://github.com/KhyatiMahendru/Dimensionality-Reduction/blob/master/Visualizations/mnist-pca-2.png)
![MNIST-SVD-2-Components](https://github.com/KhyatiMahendru/Dimensionality-Reduction/blob/master/Visualizations/mnist-svd-2.png)
![MNIST-TSNE-2-Components](https://github.com/KhyatiMahendru/Dimensionality-Reduction/blob/master/Visualizations/mnist-tsne-2.png)

### In 3 Dimensions
![MNIST-PCA-3-Components](https://github.com/KhyatiMahendru/Dimensionality-Reduction/blob/master/Visualizations/mnist-pca-3.png)
![MNIST-SVD-3-Components](https://github.com/KhyatiMahendru/Dimensionality-Reduction/blob/master/Visualizations/mnist-svd-3.png)
![MNIST-TSNE-3-Components](https://github.com/KhyatiMahendru/Dimensionality-Reduction/blob/master/Visualizations/mnist-tsne-3.png)

# Conclusion
Although tSNE was slow, it lead to the most impressive and clearly clustered visualizations in both 2D and 3D.
To reduce the time for tSNE, PCA or SVD may be used as a primary step.

