# DimensionalityReduction

## 1.Image Compression using PCA ##
In this section, A colourful image is considered. It is converted to gray scale so that RGB channel values for each pixel are summed up, then we perform PCA on the matrix and find the number of PCAs to reconsider for reconstructing an image to about 95% variance(279). I have used IncrementalPCA module from sklearn.decomposition to identify PCs, transform and represent data. It also presents a reconstructed images for different number of components for better comaprison and understanding.  
Disadvantage of PCA: If number of features are high, it is difficult to interpret PC    

## 2. Image Compression using SVD ##
In this section, a colourful image is considered. It is converted to the gray scale similar to the PCA and for similar reasons and convert the image into numpy matrix.  
To compute SVD, I have used: *np.linalg.svd()*    
Then image is reconstructed using different number of components.  

## 3. Dimensionality Reduction using LLE, t-SNE, ISOMAP, UMAP for Visual Dataset ##
In this section, I have considered a visual dataset of swiss roll (3D). I have plotted the 3D graph at first for comparison and then created a dictionary of methods of LLE, t-SNE, ISOMAP and UMAP and then plot the graph by applying all dimensionality reduction techniques
  
Working of LLE: It creates a neighbourhood graph, calculates local weight matrix for each point and use the matrix to create it's neighbour  
Disadvantageof LLE: When data is not smooth, it gives poor result  
  
Working of t-SNE: t-SNE is based on stochastic neighbor embedding(SNE).It constructs probability distributions from pairwise distances such that larger distances correspond to smaller probabilities and vice versa  
Disadvantage of t-SNE: It cannot handle dataset with higher dimension. t-SNE cannot interpret the distance between clusters  
  
Working of ISOMAP: ISOMAP computes a neighbourhood graph, adjacency matrix and dissimilarity matrix. Perfrom eigen value decomposition and choose the first K eigenvectors with K highest eigenvalues   
Disadvantage of ISOMAP: ISOMAP has poor performance when manifold is not properly sampled and contains holes
  
Working of UMAP: UMAP uses exponential probability distribution for higher dimensions. It should be able to interpret both the distances between positions of points and clusters.
Disadvanatge of UMAP: It is a new tecnique and has to be adopted  
  
## 4. Dimensionality Reduction using Tabular Dataset ##
