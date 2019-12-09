# Notebooks description

* XML2CSV: This notebook converts all of the xml files associated to each image into a single csv file we can more easily manipulate for our experiments.
* Data Split: This notebook splits the original raw data into three sets for training, validation and test.
* Etude des donnée: This notebook shows general statistics about the data we work with.
* Resize: This notebook resizes all the pictures for the specified set. It's a simple resize, the original aspect ratio of the image is not taken into account.
* Resize2: This notebook resizes all the pictures for the specified set. The method resizes the shorter side of the image to the specified value and then crops the other dimension at the center while keeping the same size for both dimensions.
* BaseLine_ClassifieursLineaires: This notebook does a naive classification, a linear classification with no image preprocessing and a linear classification using HoG features.
* Neural Networks from Scratch: This notebook defines a CNN and MLP networks and trains them from scratch.
* Neural Network Transfer Learning: This notebook performs transfer learning using ResNet18 and ResNet101 which have been pretrained on ImageNet.

# Setup

The training data can be downloaded from https://seafile.lirmm.fr/f/5d7dc75bcfbb49b991ca/?dl=1. Once it has been downloaded, it should be placed in './data/raw_data/'

1. Run XML2CSV in order to convert all the xml metadata files into a single csv
2. Execute Data Split to create the training, test and validation sets
3. Execute either Resize or Resize2 to resize the images in the 3 sets

After the initial setup has been done you can either run the linear classifiers or the deep learning models. However, dependng on which resizing method you used, you may need to change the classification notebooks to point to the right path where your images are located.

# Linear classification

1. Run HoG Features Extractor 
2. Run notebook BaseLine_ClassifieursLineaires

# Neural Networks

You can either run "Neural Networks from Scratch" or "Neural Networks Transfer Learning"
