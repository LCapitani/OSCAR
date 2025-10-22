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

Follow the steps below to set up your enviroment:

  1. Install Anaconda (https://anaconda.org)
  2. Create a conda enviroment in terminal using the command below using python 3.7.11
        conda create --name maskrcnn python==3.7.11
  3. Follow this installation guide video to clone the modified MaskRCNN repository
        https://www.youtube.com/watch?v=Fu_km7FXyaU&pp=ygUlMjg0IGRpZ2l0YWxzcmVlbmkgaW5zdGFsbGluZyBtYXNrcmNubg%3D%3D
  4. Use the **requirements.txt ** file available in this repository to install the necessary python packages
  5. To test you’ve installed everything correctly try running the command in python
        import maskrcnn
  6. MaskRCNN was further modified to be compatible with grayscale images. Replace the ‘mask_rcnn_tf2-1.0-py3.7.egg’ found at the following path ‘C:\Anaconda\envs\maskrcnn\Lib\site-packages’ with the ‘mask_rcnn_tf2-1.0-py3.7.egg’ found in this repository. If you are on mac or linux, you can find the path of the conda enviroment folder by activating the enviroment using the command

     conda activate maskrcnn

     conda info --envs
     
You should be good to go!! Feel free to raise any issues that come up on this repo :)
