# Overview

Machine Learning and Deep Learning have been transforming businesses healthcare and medicine. Deep Learning specifically has been proven to be superior to detect and classify diseases by using imagery data.

In this project, I leverage Kera's API to apply deep learning skills to improve disease detection processes such as Convolutional Neural Networks and Residual Neural Networks (resNet). Then train a resNet model to perform image classification by using transfer learning, as well as use Confusing 
Matrix to evaluate performance of the model.

The purpose of this project is to achieved automatically detecting and classifying different types of chest diseases such as healthy, covid-19, bacterial pneumonia, and viral pneumonia based on X-ray images, which can help a doctor to determine a chest disease case in a short time.
  - Model testing validation accuracy: 80% with 50 epochs.
  - The model has weak performance at precision for covid-19 & bacterial pneumonia symptoms with 68% & 55% accuracy.


### Problem Statement

In this case, I am a deep learning consultant that work at a hospital in New York City. Recently, I have been tasked to develop a model by using extensive chest X-ray images to automate the process of detecting and classifying different types of chest disease, as well as reduce the cost and time of detection. The chest diseases were classified as Healthy, Covid-19, Bacterial Pneumonia and Viral Pneumonia.


### Data:

  https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia
  
  
### Methodology:

  - Data visualization
  <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Chest_Disease_Classification/images/1.png" width="600" height="400"> 
   
   
### Modeling:

  - Download residual network Model as a based model for this project
    - Import pre-trained model with weights
    - Freezing some layers of the based model, which we don't want them to change
    - Build and train a new model to fit this project
      - Build a new fully-connected model
      - To see how the new model work with training data
  <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Chest_Disease_Classification/images/2.png" width="600" height="400"> 
  
  <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Chest_Disease_Classification/images/3.png"> 
  
  - Evaluation of training data
    - Accuracy
    - Loss
    - Validation Accuracy
    - Validation Loss
  <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Chest_Disease_Classification/images/4.png" width="600" height="400"> 
  
  <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Chest_Disease_Classification/images/5.png" width="600" height="400"> 
  
  <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Chest_Disease_Classification/images/6.png" width="600" height="400"> 
  
  <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Chest_Disease_Classification/images/7.png" width="600" height="400"> 

  
### Results:

  - Model highest training validation accuracy: 93.27%
  - Model testing validation accuracy: 80%
  <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Chest_Disease_Classification/images/8.png" width="600" height="500">


### Evalution Metric

  - Confusion matrix
  <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Chest_Disease_Classification/images/9.png" width="400" height="150">
  <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Chest_Disease_Classification/images/10.png"  width="600" height="400">


### Conclusions:

  80% accuracy in prediction is acceptable result in this case since I only using 428 images to train the model. It also tell us hunman's intervention is necessary   even though a model has a high accuracy. The evalution report tells us that the model is weak at the Covid-19 chest disease prediction, which with 64% accuracy   precision rate, and also is weak at the bacterial pneumonia chest disease prediction, which with 50% accuracy recall rate. I think there are two main reasons cause   this situation, first, the dataset too small, which only has 428 images for training and 104 images for testing. Secondly, this is a pre-trained resNet model, I  just using the original weights of this model. I believe that if I can re-build a new model from scratch, it should perform better, but it may need a big dataset.
