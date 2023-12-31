 
## Corn Detect [Recognition of Corn Diseases by Leaf Image Classification]

 
## Description

 The versatile Corn Detect app runs seamlessly on all devices, including mobile phones, laptops, and tablets. Whether you're in the field or at your desk, you can easily access and utilize the app's powerful disease detection capabilities. Our user-friendly interface ensures a consistent and optimized experience across various platforms, empowering farmers to detect and manage diseases in corn crops conveniently, regardless of the device they prefer to use. With Corn Detect, you have the flexibility to monitor and safeguard your crops anytime, anywhere.

   <img src="./Assets/Screenshot 2023-07-10 121741.png" alt="models" />




## Leaf Image Classification

  <img src="./Assets/features.png" alt="models" />
  This project is an approach to the development of corn disease recognition model, based on corn leaf image classification, by the
use of deep convolutional networks. <br>
   <br> <img src="./Assets/case.png" alt="models" />
    The developed model is able to recognize 4 different types of corn diseases.
<br>
 <img src="./Assets/predict.png" alt="models" />
 <br>
1. Data gathering

   The dataset taken was **"kaggle"**. It can be downloaded through the link "https://www.kaggle.com/datasets/buffyhridoy/corn-disease". It is an Image dataset containing images of different healthy and unhealthy crop leaves.

   The dataset wasn't enough so I did a bit of data augmentation to expand the number of datasets from 5000 to 10,000.

   After augmenting I did data spliting, i.e 70% for training, 20% testing and 10% for validation.

3. Model building

   - I used pytorch for building the model ON google collab.
   - I develope a custome CNN model consisting of three convolutional layer, three max pool layer and three fully connceted layer. The system don't only predict the diseases it also add the causes and relevant solutions.  

4. Training

   The model was trained by using variants of above layers mentioned in model building and by varying hyperparameters. The best model was able to achieve 94.76% of test accuracy and 89.89% of validation accuracy.

5. Testing

   The model was tested on total 10,000 images of 4 classes.<br/>
   The model used for prediction on sample images. It can be seen below:
   <!-- <img src="" alt="index1" height="300px"/> -->
   <div>
  
   </div>

6. Various Model Architecture tried along with Learning Rate and Optimizer and various accuracy obtained with different models.

 
 <br/>
 

## Further Work:

- Implementing Image Localisation to find the excat position of the leaf affected .
- Building Recommender system for recommendation of proper presticides and control method for the disease.
- Implementing the appropriate management strategies like fungicide applications and pesticide applications could lead to early
  information on crop health and disease detection.This could facilitate the control of diseases and improve productivity.

## Usage:

- `Flask` : Code for Flask Server and deployment
- `TestImages` : Sample image for model testing
- `Src` : All The source code for building models
- `Models` : All the Pretrained Models of Pytorch


 
