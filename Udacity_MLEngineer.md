---
title: "Udacity_MLEngineer"
author: "Aman Jindal"
---

### A. Project 1: Building a Movie Review Sentiment Classifier

The following are the key learnings:

1. Building and training a LSTM Network (100 cell single layer) using PyTorch. <a href="https://pythonprogramming.net/training-deep-learning-neural-network-pytorch/" target="_blank">This link</a> explains the basics of making a model with PyTorch.
2. AWS SageMaker.
3. Deploying the ML Model.
4. Building an AWS Lambda Function.
5. Building an AWS API Gateway.
  
### B. Project 2: Population Segmentation using SageMaker

The following are the key learnings:

1. **AWS SageMaker Ground Truth:** Helps in going from raw data, to labelled data. It first sends the data to humans for initial labels. Then it trains an ML model based on these initial labels, to automate the labelling process. 
2. Kernel to use: co.nda_mxnet_p36 or conda_pytorch_p36 ; p36 denotes python version 3.6 
3. <a href="https://docs.aws.amazon.com/sagemaker/latest/dg/deepar_how-it-works.html" target="_blank">DeepAR</a> is an inbuilt Supervised Learning model (a RNN) in Sagemaker for Time Series data.  
4. Calculated two different kind of features viz. containment and longest common subsequence (lcs) for the answer & source texts.
5. Categorized text as plagiarized or not using a random forrest classifier.

### C. Project 3 and 4: Dog Breed CNN (Convolutional Neural Network) Classifier

The following are the key learnings:

- To identify the breed of a dog, built two different CNN algorithms viz. <br>

  1. Built a CNN Algorithm from scratch to identify dog breed from 133 dog breeds.
  2. Used <a href="https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html" target="_blank">Transfer Learning</a> to build the dog breed classifier. ResNet-18 model was used whose last fully connected layer was replaced by a 133 neuron fully connected layer. Only the last layer was trained. <br>
   

- Additionally: <br>
     
  1. Used <a href='https://docs.opencv.org/master/db/d28/tutorial_cascade_classifier.html' target="_blank">Haar feature based cascade classifier provided by OpenCV</a> to detect human faces in an image.
  2. Used a pre-trained <a href="https://pytorch.org/vision/stable/models.html" target="_blank">VGG-16 from torchvision.models</a> to detect a dog in an image. VGG-16 has been trained on the ImageNet Dataset whose classes 151 to 268 correspond to dogs. Thus, an output within this range implies the image is of a dog. 