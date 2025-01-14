# OSCAR: An Online ML-Powered Tool for Organoid Cell Counting using Brightfield Images 

![Logo](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTilnfd7wntKPiGUlI2gp2Q5dYw6at1VVzeaQ&s)

## Description

Here you can find the code, and directions to relevant raw images, data and models that went into the creation of OSCAR (Organoid Segmentation and Cell number Approximation using Regression), a two-step workflow capable of estimating organoid cell numbers from brightfield microscopy images. The first step is a Mask RCNN-based convolutional neural network capable of identifying organoids in brightfield microscopy images and generating an estimate of the area of each organoid in the image. The second step is an empirical multiple linear regression model relating the number of cells in an organoid to the area of the organoid estimated by the Mask RCNN model. 

Raw data (and accompaning meta data) and developed models are available on Open Science Framework [here.](https://osf.io/ehdtk/)

## Features

- MASK R-CNN publication ready.ipynb  contains python code in Jupyter Notebook format used to develop train and test the MaskRCNN model
- eMLR publication ready.ipynb contains python code in Jupyter Notebook format used to develop train and test the emperical multiple linear regression model
- Model locattions.txt contains instructions on how models can be downloaded and accessed

## Access

We make OSCAR free to use in an easily accessible format as a Google Colab notebook, where anyone, regardless of coding sklls, can upload organoid images and obtain organoid cell number estimates.

[OSCAR can be accessed here.](https://colab.research.google.com/drive/1paRiDvvAu4ezZEesSdUH-fO_BJ8eJgsY?usp=sharing)

## Citation

If you use OSCAR and publish any work in which it was involved, please cite our work:
*PAPER CITATION TO BE INSERTED.*
