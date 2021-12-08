# DetectX-Accident-Detection-Using-Deep-Learning
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
[![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/Naereen/StrapDown.js/blob/master/LICENSE)
# Overview 
Our main goal of this project is to use deep learning and computer vision to detect accidents on dashcam and other visual footages that can be utilized ,and to report it to nearby emergency services with valid accident images.
# Challenges
1. To design a deep convolutional neural networks model for this project.

2. Limited hardware resorces like GPU's.

# Model Overview

DenseNet was developed specifically to improve the declined accuracy caused by the vanishing gradient in high-level neural networks. In simpler terms, due to the longer path between the input layer and the output layer, the information vanishes before reaching its destination.
An output of the previous layer acts as an input of the second layer by using composite function operation. This composite operation consists of the convolution layer, pooling layer, batch normalization, and non-linear activation layer.

These connections mean that the network has L(L+1)/2 direct connections. L is the number of layers in the architecture.

The DenseNet has different versions, like DenseNet-121, DenseNet-160, DenseNet-201, etc. The numbers denote the number of layers in the neural network. The version we tweak is Densenet-161 architecture.
DenseNets have several compelling advantages: 
              they alleviate the vanishing-gradient problem, strengthen feature propagation, encourage feature reuse, and substantially reduce the number of parameters.
The 1-crop error rates on the imagenet dataset with the pretrained model are listed below.

Model structure    Top-1 error    Top-5 error

densenet121  :  25.35   : 7.83

densenet169  :  24.00   : 7.00

densenet201  :  22.80   : 6.43

densenet161  :  22.35   : 6.20

![alt text](https://raw.githubusercontent.com/arjunks2112/DetectX-Accident-Detection-Using-Deep-Learning/master/assets/densenet.png)

![alt text](https://raw.githubusercontent.com/arjunks2112/DetectX-Accident-Detection-Using-Deep-Learning/master/assets/arch.png)
 
![alt text](https://raw.githubusercontent.com/arjunks2112/DetectX-Accident-Detection-Using-Deep-Learning/master/assets/block.png)

# Required Modules

webbrowser
torch
num as py
cv2(opencv)
torchvision
dlib

# Prerequisite 

Download anaconda from here https://www.anaconda.com/distribution/#download-section

1. Pytorch 

> conda install pytorch torchvision cudatoolkit=10.1 -c pytorch


2. OpenCV 

> conda install -c conda-forge opencv
