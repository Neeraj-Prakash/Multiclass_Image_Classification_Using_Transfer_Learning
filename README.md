# Multiclass Image Classification Using Transfer Learning

Classifying images of 6 different classes of images using Transfer Learning in Keras using Tensorflow backend

The Dataset I used can be downloaded from this [**link**](https://www.kaggle.com/puneet6060/intel-image-classification)

I used the **"Google Colab"** platform to run this project. It is very convenient, as it provides a GPU to train Deep Learning models for free.

## The Problem
The given dataset contains images that belong to **six** different classes. The classes are as follows: 
- Buildings
- Forest
- Glacier 
- Mountain
- Sea
- Street
  
We need to train a model that can classify these images with high confidence.  

## The Model  
I chose the **InceptionV3** model to train on the given dataset.  
I chose it because it is **faster** than models like VGG or Resnet. And It **more accurate** compared to MobileNet.  
The paper for the InceptionV3 model can be found in this [link](https://arxiv.org/abs/1512.00567)

I used **Transfer Learning** in this project, i.e., I downloaded the inceptionV3 network trained on 'ImageNet' dataset and froze the hidden layers.
I created last 2 layers as per my requirement and trained those layers with the given data. 
Here is a good introduction to "Transfer Learning" by Andrew NG. [Link](https://www.youtube.com/watch?v=yofjFQddwHE&t=2s)
  
  
## Evaluating Model
The trained model was evaluated on the 'Test set', which was not included in the training. 
The model gets around **89%** of accuracy in the given set.  

I also predicted the labels on unlabled images in the given dataset using my trained model.  
  
Do check out the code to get more details and understand the project.
