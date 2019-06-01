## Project: Build a Traffic Sign Recognition Program
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

Overview
---
In this project, we will use deep neural networks and convolutional neural networks to classify traffic signs. We will train and validate a model so it can classify traffic sign images using the [German Traffic Sign Dataset](http://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset). After the model is trained, we will then try out your model on images of German traffic signs that we find on the web.

Data Files
---

* the Ipython notebook with the code - Traffic_Sign_Classifier.ipynb
* the code exported as an html file - Traffic_Sign_Classifier.html
* Github: https://github.com/SmokeShine/CarND-Traffic-Sign-Classifier-Project/

Logic
---
The steps of this project are the following:
* The raw data is loaded from the pickle files
* We found the data is not unbalanced and all the labels are present in similar proportion across the train, test and validation dataset. This implies the data is sampled from the same distribution for creating the three datasets
* For pre processing, we are converting the image to gray scale and then normalizing using a min max scalar
* For the architecture, we are using the LeNet architecture with Xavier initializtion
* Optimizer is adam, while the loss function is cross entropy loss.
* The model is trained with the following hyper parameters
** EPOCHS = 30
** BATCH_SIZE = 32
** rate = 0.0009
* The validation accuracy is closed to 93%, while the test accuracy is 92%
* For custom images downloaded from the image, the accuracy is 75%, implying the new images are indeed selected may be different from the images trained on

### Dependencies
This lab requires:

* [CarND Term1 Starter Kit](https://github.com/udacity/CarND-Term1-Starter-Kit)

The lab environment can be created with CarND Term1 Starter Kit. Click [here](https://github.com/udacity/CarND-Term1-Starter-Kit/blob/master/README.md) for the details.

