# CNN-image-classification
This project aims to make medical image classification models using Convolutional Neural Network (CNN) built with Pytorch. Four different classification tasks have been tried out: Pneumonia, Covid-19, brain tumors, and retinal OCT. The codes follow the same architecture, with the datasets altered. The repository contains jupyter notebooks for the trials.

## Details
The structre of the CNN is based on the Pytorch tutorial (https://docs.pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html). The images in the datasets are resized to 32x32 pixels. The CNN consists of two convolutional layers with 5x5 kernel, two max pooling layers, and three fully connected layers. Between the layers, ReLU function is used as the activation function to introduce non-linearity. Each project achieved ~70-85% accuracy depending on the number of epochs. Further improvements can be achieved by optimising the hyperparameters.

## References & Acknowledgements
### Datasets used:
https://www.kaggle.com/datasets/pranavraikokte/covid19-image-dataset  
https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia  
https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset  
https://www.kaggle.com/datasets/paultimothymooney/kermany2018

  
### Codes modified and adapted from:
https://www.youtube.com/watch?v=ZBfpkepdZlw  
https://www.youtube.com/watch?v=CtzfbUwrYGI  
https://docs.pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html  

### Other resources referenced:
https://qiita.com/momoyama/items/aecf831fbf887f067d42  
https://www.youtube.com/watch?v=igQeI29FIQM  
https://qiita.com/Nari_Lefty/items/adc1fce73cb59ac01ab4  
https://zenn.dev/hirayuki/articles/bbc0eec8cd816c183408  
https://qiita.com/ssc-nurabe/items/a3e5c9e5255f526a2977  
  

