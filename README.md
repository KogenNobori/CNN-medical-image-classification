# CNN Medical Image Classification
This project aims to develop medical image classification models using Convolutional Neural Networks (CNNs) built using PyTorch. Four different classification tasks using public datasets on Kaggle were tried out: Pneumonia, Covid-19, brain tumors, and retinal OCT. The code follows the same architecture, with the datasets altered. The repository contains jupyter notebooks for the trials. The notebooks have been confirmed to run successfully in Google Colaboratory.

## Neural Network
The structure of the CNN is based on the [PyTorch tutorial](https://docs.pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html). The image inputs from the datasets are resized to 32x32 pixels in preprocessing. The CNN consists of two convolutional layers with a 5x5 kernel, two max pooling layers, and three fully connected layers. Between the layers, the ReLU function is used as the activation function to introduce non-linearity. The cross-entropy loss is used as the loss function, and optimization is done by Stochastic Gradient Descent, which is supported by Autograd in PyTorch.

## Classification tasks
The classes the model aimed to identify in each dataset are as follows:  

Pneumonia　&nbsp;... normal, Pneumonia;  
Covid-19 &nbsp; &nbsp; &nbsp;... normal, Covid-19, viral Pneumonia;  
Brain tumors ... Glioma, Meningioma, Pituitary tumor, no tumor;  
Retinal OCT &nbsp;... normal, CNV, DME, drusen  

Each project achieved **70-85%** accuracy depending on the number of epochs. 

## Analysis
Although improvements are essential, the 70-85% accuracy is promising, especially for the tasks with four or five classes, considering the small computational resources used. In this project, the model was run on T4 GPU (or CPU when it is unavailable) on Google Colaboratory. In order to reduce the time taken for training, the images in the datasets are resized to 32x32 pixels. However, the accuracy may be improved by using higher-resolution images (e.g., 256x256), which will require more computational resources. Further improvements can be achieved by optimizing the hyperparameters (such as learning rate, number of epochs, batch size, depth of different kinds of layers, etc.)


## References & Acknowledgements
### Datasets used:
[Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)  
[Covid-19 Image Dataset](https://www.kaggle.com/datasets/pranavraikokte/covid19-image-dataset)  
[Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)  
[Retinal OCT Images (optical coherence tomography)](https://www.kaggle.com/datasets/paultimothymooney/kermany2018)

  
### Code modified and adapted from:
[Convolutional Neural Nets Explained and Implemented in Python (PyTorch)](https://www.youtube.com/watch?v=ZBfpkepdZlw)  
[Image Classification CNN in PyTorch](https://www.youtube.com/watch?v=CtzfbUwrYGI)  
[PyTorch tutorial](https://docs.pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html)  

### Other resources referenced:
https://qiita.com/momoyama/items/aecf831fbf887f067d42  
https://www.youtube.com/watch?v=igQeI29FIQM  
https://qiita.com/Nari_Lefty/items/adc1fce73cb59ac01ab4  
https://zenn.dev/hirayuki/articles/bbc0eec8cd816c183408  
https://qiita.com/ssc-nurabe/items/a3e5c9e5255f526a2977  
  

