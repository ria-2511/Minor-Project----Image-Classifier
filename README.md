# INTRODUCTION
This is an Image Classifier using K Nearest neighbors in SK Learn. 
We have chosen a few Categories of images and then have made a dataset with the help of those images. Further analysis of that dataset is done and a final model is created using the KNN Algorithm (Details Below). This model can now predict images of the category was fed earier.

Dataset Folder Link : https://drive.google.com/drive/folders/1-OYmxffUDVE3LkStjeG_ysp9hLFZDVv2?usp=sharing

## Algorithm Used 
The Machine Learning Algorithym that I have used here is K- Nearest Neighbors. 

It is a type of **supervised machine learning** algorithm. A supervised machine learning algorithm (as opposed to an unsupervised machine learning algorithm) is one that relies on labeled input data to learn a function that produces an appropriate output when given new unlabeled data. Supervised machine learning algorithms are used to solve classification or regression problems. A **classification problem** has a discrete value as its output. For example, “likes pineapple on pizza” and “does not like pineapple on pizza” are discrete. There is no middle ground. 
The KNN algorithm assumes that similar things exist in close proximity. In other words, similar things are near to each other.

“Birds of a feather flock together.”

<img src="https://miro.medium.com/max/611/1*wW8O-0xVQUFhBGexx2B6hg.png">

Notice in the image above that most of the time, similar data points are close to each other. The KNN algorithm hinges on this assumption being true enough for the algorithm to be useful. KNN captures the idea of similarity (sometimes called distance, proximity, or closeness) with some mathematics we might have learned in our childhood— calculating the distance between points on a graph. 

There are vaious ways to calculate the distance for this Algorithm . Euclidean distance is the most popular distance metric. You can also use Hamming distance, Manhattan distance, Minkowski distance as per your need.

In my Project I have used the MINKOWSKI distance (since that is the default distance set). The Minkowski distance between two variabes X and Y is defined as

**(∑i=1n|Xi−Yi|p)1/p** 

The case where p = 1 is equivalent to the Manhattan distance and the case where p = 2 is equivalent to the Euclidean distance. In my project , p=2 (also set default) i.e. I have used the Euclidean Distance.

## Steps / Work Done 
* Import the libraries needed 
* Create a directory to save the said images 
* Install Bing Image Downloader and further Download Images of 3 categories (vegetables)
* Flatten ans resize the images 
* Append them into a new list named TARGET 
* Using Pandas create a dataframe of the flattened images 
* Divide this dataset into train and test dataset with a ratio of 8:2 
* Apply K-Nearest Neighbors and create a model which can succesfully classify the images 
* Check the model on a new dowloaded image dataset 
* Display the Evaluation metrics of the model 

## Results 
* Accuracy - 69% 
* Confusion Matrix - array([[2, 1],[0, 0]])

## Scope for Imporvement
* We can increase the size of the dataset by taking more images and that too of new categories. 
* Various Other Classification Algorithms can also be used here to increase the accuracy of the model 

## Bibliography 
* https://www.javatpoint.com/k-nearest-neighbor-algorithm-for-machine-learning
* https://www.pyimagesearch.com/2016/08/08/k-nn-classifier-for-image-classification/
* https://towardsdatascience.com/machine-learning-basics-with-the-k-nearest-neighbors-algorithm-6a6e71d01761
* https://www.analyticsvidhya.com/blog/2021/04/simple-understanding-and-implementation-of-knn-algorithm/
* https://www.geeksforgeeks.org/k-nearest-neighbours/
