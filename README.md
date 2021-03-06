## Identifying Cat and Dogs based on CNN Model

## Introduction
The project aims to  identify the Cat and Dogs based on a Deep Learning Model. I am using Convolutional Neural Network (CNN) to identify the characteristics between Cat and Dogs. Several steps are needed to identify the classification, which are : 

- Import All Libraries
- Loading the Dataset (Cats and Dogs) 
- Image Data Generator 
- Define the parameters using Convolutional Neural Network (CNN) Model
- Compiling CNN to the model 
- Plotting the Losses and Validation Losses
- Evaluating the Model
- Creating Dataframe Dog and Cat columns
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
What is the Maximum Pooling? It is basically the downsampling strategy in CNN, to reduce its dimensionality, we need to find the  
- ##### Dropout #####
The dropout reduces the **overfitting** model by ignoring some units during modelling phase. 
- ##### Flatten #####
The Flatten reshapes the existing dimension into *(:,1,:)*, which is used for next step of the Neural Network.

### 5. Compiling the CNN to the model
In this section, this research defines Three paramters ; *Batch Size* , *Model Compiler*, and the *Model Fit Generator*. 
- Mini-Batch Size : 2 
- Model Compiler : We are using 'Adam' Optimizer with a loss calculation 'Binary Crossentropy' with a metrics 'Accuracy'. The Binary Crossentropy returns only 1 classification, however, we may use a probability to detect the Cat and Dog Classifiaction. 
- Model Fit Generator : We are using 50 number of epochs running smoothly through the neural network. 

### 6. Plotting the Losses and Validation Losses
A basic matter to plot the Losses and Accuracy

### 7. Evaluating the Model
After compiling the Model to the Dataset, we will evaluate the model and deploy how much accuracy after being tested to the Validation Dataset. 

### 8. Creating Dataframe of Cat and Dogs
A basic function to deploy a simple column of Cat and Dogs 

### 9. Predicting the Cat and Dog 
A Model Prediction to the Validation Dataset
