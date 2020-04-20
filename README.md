# Identifying Cat and Dogs based on CNN Model

# Introduction
The project aims to  identify the Cat and Dogs based on a Deep Learning Model. I am using Convolutional Neural Network (CNN) to identify the characteristics between Cat and Dogs. Several steps are needed to identify the classification, which are : 

- Import All Libraries
- Loading the Dataset (Cats and Dogs) 
- Image Data Generator 
- Deploy the Convolutional Neural Network (CNN) with several parameters
- Compiling CNN to the model 
- Plotting the Losses and Validation Losses
- Predicting the Cat and Dog 

We will discuss this one by one : 

## 1. Import all libraries needed 
Basically, we need a basic deep learning library (TensorFlow) and also the Matlab library (for plotting).
---
# Import all libraries needed
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import tensorflow as tf
import math

from PIL import Image
import PIL
# Import All Images Libraries
from matplotlib import pyplot
from matplotlib.image import imread
---
