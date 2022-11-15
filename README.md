# **ENEE633/CMSC828C**

<p>
The aim of this project is to implement different classifiers to achieve face recognition. You are
given a set of faces and their corresponding labels. You need to split the data into training and
testing sets and use the training data to train your classifiers. The whole pipeline is described in
the following section.
</p>

#### Classifiers implemented:
1. Bayes’ Classifier
2. KNN
3. Kernel SVM
4. Boosted SVM

#### Dimensionality reduction methods implemented:
1. PCA
2. MDA

#### Dataset:
data.mat

	200 subjects
	3 faces per subject
	size: 24 x 21

	The file 'data.mat' has a variable ”face” of size (24x21x600). The images corresponding to the
	person labeled n, n = {1, . . . , 200}, can be indexed in Matlab as face(:,:,3*n-2), face(:,:,3*n-1)
	and face(:,:,3*n). The first image is a neutral face, the second image is a face with facial
	expression, and the third image has illumination variations.

pose.mat

	68 subjects
	13 images per subject (13 different poses)
	size: 48 x 40

	The file 'pose.mat' has a variable "pose" of size 48x40x13x68. 
	pose(:,:,i,j) gives i^th image of j^th subject.


illumination.mat

	68 subjects
	21 images per subject (21 different illuminations)
	size: 48x40

	The file 'illumination.mat' has a variable "illum" of size 1920x21x68.
	reshape(illum(:, i,j), 48, 40) gives i^th image of j^th subject.


