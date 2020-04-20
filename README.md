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
- Validation

### 3. Image Data Generator 
In this part, we are defining the train and test dataset based on the dataset load. We build a Data Generator which aims to reschale the model. 

### 4. Define the parameters using Convolutional Neural Network (CNN) Model
We are using the basic convolutional model 2D (CNN), which consist of : 

- ##### Convolutional #####
   
- ##### BatchNormalization #####
This is mainly used for normalizing the activation function of the previous layer for each batch. Basically, this provides of reparameterizing almost any deep neural network. This technique also called as Whitening
- ##### Maximum Pooling #####
What is the Maximum Pooling? Well, it is basically the downsampling strategy in CNN, which also aims to reduct its dimensionality. 
- ##### Dropout #####
The dropout means dropping a sample of dataset which aims to reduce the **overfitting** by ignoring some units, during the training phase. 
