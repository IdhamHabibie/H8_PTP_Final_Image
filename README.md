## Identifying Cat and Dogs based on CNN Model

## Introduction
The project aims to  identify the Cat and Dogs based on a Deep Learning Model. I am using Convolutional Neural Network (CNN) to identify the characteristics between Cat and Dogs. Several steps are needed to identify the classification, which are : 

- Import All Libraries
- Loading the Dataset (Cats and Dogs) 
- Image Data Generator 
- Define the parameters using Convolutional Neural Network (CNN) Model
- Compiling CNN to the model 
- Plotting the Losses and Validation Losses
- Predicting the Cat and Dog 

We will discuss this one by one : 

### 1. Import all libraries needed 
Basically, we need a basic deep learning library (TensorFlow) and also the Matlab library (for plotting). We also need Keras Library to identify the CNN model. 

### 2. Loading the Dataset
I put the library on the **cats_and_dogs_filtered/cats_and_dogs_filtered/**, which consist of two folders : 
- Train
- Validation (Testing Data) 
In section 3, the Image Data Generator will classify the classes inside the Train and the Validation. 

### 3. Image Data Generator 
In this part, we are defining the train and test dataset based on the dataset load. We build a Data Generator which aims to rescaling  the model. 

### 4. Define the parameters using Convolutional Neural Network (CNN) Model
CNN is one of the Neural Network method that uses convolution method. But what is the Convolution? In terms of Signal and Processing, the convolution defines a way of combining two signals to create the third signal, by doing convolution. For example if you have **f** and **g** as a function, the **g** function will multiply with **f** by creating windowing method. On the other hand, the convolution formula is the integral of **f** multiplies with the inverse of **g**, which results a third signal.  

We are using the basic convolutional model 2D (CNN), which consist of : 

- ##### Convolutional #####
The layer of the images are convoluted into the next layer, which aims to have a feature extraction. 
- ##### BatchNormalization #####
This is mainly used for normalizing the activation function of the previous layer for each batch. Basically, this provides of reparameterizing almost any deep neural network. This technique also called as Whitening
- ##### Maximum Pooling #####
What is the Maximum Pooling? Well, it is basically the downsampling strategy in CNN, which also aims to reduct its dimensionality. 
- ##### Dropout #####
The dropout means dropping a sample of dataset which aims to reduce the **overfitting** by ignoring some units, during the training phase. 
- ##### Flatten #####
The Flatten reshapes the existing dimension into (:,1,:), which aims to be calculated for the Neural Network.
