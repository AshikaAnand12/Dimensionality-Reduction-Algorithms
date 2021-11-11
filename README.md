# DimensionalityReduction

##1. Image Compression using PCA##
In this section, A colourful image is considered. It is converted to gray scale so that RGB channel values for each pixel are summed up, then we perform PCA on the matrix and find the number of PCAs to reconsider for reconstructing an image to about 95% variance(279). I have used IncrementalPCA module from sklearn.decomposition to identify PCs, transform and represent data. It also presents a reconstructed images for different number of components for better comaprison and understanding.
Disadvantage of PCA: If number of features are high, it is difficult to interpret PC
- - - -
##2. Image Compression using SVD##
- - - -
##3. Dimensionality Reduction using LLE, t-SNE, ISOMAP, UMAP for Visual Dataset##
- - - -
##4. Dimensionality Reduction using Tabular Dataset##
