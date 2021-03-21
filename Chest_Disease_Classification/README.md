# Chest Disease Classification

  This project used deep learning technique in healthcare industry and achieved automaticly detecting and classifying to different types of chest diseases such as healthy, covid-19, bacterial pneumonia and viral pneumonia by using chest X-ray images, which can help a doctor to determine a chest disease case in short time.
  - Applied Keras' API to build a convolutional networks
  - Applied residual neural network for transfer learning
  - Evaluated resNet training model on test data
  - Applied confusion metric for precision and recall


### Background

  AI/ML/DL has been revolutionizing in industries of healthcare and medicine, such as medical imagery, drug research and genome development. Also, it has been aproven to be superior in detecting and classifying disease using imagery data. For example, skin cancer could be detected more accurate by deep learning than by dermatologists in 2018.
  - Human dermatologists detection is 86.6%
  - Deep learning detection is 95%
  - Reference: "Computer learns to detect skin cancer more accurate than doctors". The Guardian, 29 May 2018


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
    <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Chest_Disease_Classification/images/2.png" width="600" height="400"> 
    - Freezing some layers of the based model, which we don't want them to change
    - Build and train a new model to fit this project
      - Build a new fully-connected model
      - To see how the new model work with training data
  - Evaluation of training data
    - Accuracy
    - Loss
    - Validation Accuracy
    - Validation Loss

  
### Results:

  - Model highest training validation accuracy: 93.27%
  - Model testing validation accuracy: 80%


### Evalution Metric

  - Confusion matrix


### Conclusions:

  80% accuracy in prediction is acceptable result in this case since I only using 428 images to train the model. It also tell us hunman's intervention is necessary even though a model has a high accuracy. The evalution report tells us that the model is weak at the Covid-19 chest disease prediction, which with 64% accuracy precision rate, and also is weak at the bacterial pneumonia chest disease prediction, which with 50% accuracy recall rate. I think there are two main reasons cause this situation, first, the dataset too small, which only has 428 images for training and 104 images for testing. Secondly, this is a pre-trained resNet model, I just using the original weights of this model. I believe that if I can re-build a new model from scratch, it should perform better, but it may need a big dataset.
