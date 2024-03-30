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

**NOTE:** Bounadry unfolding approach is based on countour detection and calculation of distances from the centroid to each boundary point
the input image is the convered binary image.

CNN Classification Model ![Uploading Binary image with contour detection.png…]()

--------------------------------
A CNN model is built for classifying tree images based the similarity between the images. The CNN was trained using natural tree datset where the images were labeled and divided into seven clusters:
0- Columnar
1- Irregular
2- Open 
3- Oval
4- Pyramidal
5- Round
6- Spreading

Example
--------------------------------


![Result Plot of Example](example/example.png)
