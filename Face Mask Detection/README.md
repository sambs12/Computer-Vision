# Face-Mask-Detection

## Problem Statement
To detect whether a person is wearing a face-mask or not by using CNN and OpenCV

## Dataset 
Dataset consists of 7553 RGB images in 2 folders as withmask and withoutmask. Images are named as label withmask and withoutmask are distibuted in 2 folders namely 
1. `without_mask` - which contains 3828 images without mask.
2. `with mask`- which contains  3725 images with masks.

1776 images including both With and Without Face Mask images from Prajna Bhandary's Github account
https://github.com/prajnasb/observations

Remaining 5777 images are collected and filtered from Google search engine.

One can download the complete dataset from https://www.kaggle.com/omkargurav/face-mask-dataset

## Image Preprocessing

It's difficult to find images of same size, and Neural Networks expects images of a fixed size.
Therefore I have performed the following preprocessing steps on all the images
1.  Normalize
2.  Resize
3.  Reshape


## Model Building and Training :
1.  I have created a basic model using CNN and Keras library.
2.  The model is trained on both **with and without masks images**.
3.  Then the model is tested on sample test data.Once the model gives a good accuracy, that is saved and used for detecting the face mask in live situation.



## Model Prediction

1. The model that gives best accuracy both on test and train dataset is saved.
2. Using webcam we are generating the test images and predicting whether the person is wearing a mask or not..

