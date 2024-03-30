# Tree-Shaped Network Similarity Measure
====================================

This repository contains the source code for tree-shaped similarity algorithm developed by [Mona A. Ahmed, Omar M. Salim, Mahmoud Adel Hassan, Hassen Taher Dorrah, Walaa Ibrahim Gabr. 2024]. The algorithm is based on morphological and outer shape of tree networks


**NOTE:** The dataset of three-order tree-shaped network is recorded in an excel sheet


Similarity Algorithm
--------------------------------

The tree-shaped similarity algorithm consists of seven steps:

1. Analyze morphological characteristics of tree network
2. Compute three morphological-based bifurcation ratios
3. Calculate overall inner arithmetic and geometric degrees of similarities 
4. Reading, preprocessing, and Filtering the input image for outer feature extraction
5. Detecting contour of binary tree network
6. Apply invariant moment technique and boundary unfolding approach for outer similarity analysis


CNN Classification Model
--------------------------------
A CNN model is built for classifying tree images based the similarity between the images. The CNN was trained using natural tree datset where the images were labeled and divided into seven clusters:
0- Columnar
1- Irregular
2- Open 
3- Oval
4- Pyramidal
5- Round
6- Spreading

Convert image binary Image and detect contour
--------------------------------
The source code for this conversion is in file "BinaryImageConversionandInvariantMomentsTechnique.ipynb"

#Input image 
![Input image](https://github.com/3mona/Tree-Shaped-Similarity-methods/assets/123502514/e8d10930-5b51-4eda-9d3a-6d0046bce868)

#Binary image
![Binary image with contour detection](https://github.com/3mona/Tree-Shaped-Similarity-methods/assets/123502514/365c67f2-6822-4be7-aa71-1be455f406a4)

Boundary unfolding transformation process
------------------------------
Bounadry unfolding approach is based on countour detection and calculation of distances from the centroid to each boundary point.
the input image is the convered binary image.
An example of a tree-shaped network shown in (a) where the boundary is divided into 360 points. The shape is transformed to an unfolded graph (b) and then the autocorrelation function is calculated as presented in (c) 
![Tree-shaped watershed network](https://github.com/3mona/Tree-Shaped-Similarity-methods/assets/123502514/103776ad-f86f-4d2b-8105-74171b579d92)

