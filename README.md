# Dl-HAR
Time series Analyses for Deep Learning based Human Activity Recognition

Human Activity Recognition (HAR) is a field of study that focuses on the spontaneous recognition of
people’s daily routine activities by utilizing time series recordings made using sensors( 1 ). We are
using labelled data from basketball players’ activities in our HAR investigation

# Data Pre-Processing
The data for all the players is imported. This data is first cleaned. The cleaning process includes
removing not_labelled values, correcting incorrect labels.

![image](https://user-images.githubusercontent.com/105876342/184662002-817070a2-530f-42a6-8dc5-56de485e24ac.png)

# Training Model

The processed data was then trained using the following models. We experimented with 3 different
Models using Pytorch. All the models were trained using the 80:20 approach only.The pytorch model was used for Basketball layer only. The models are as follows:

    • Single LSTM Model 
    • Double Stacked LSTM Model
    • ResNet (Transfer learning model) 

Using TensorFlow, we used only 1 model but we had three approaches. The model is similar to the Single LSTM model. The TensorFlow model was used for the **Basketball layer and Locomotion Layer**. The three approaches for the model are:
    
    • 80:20 Split
    • K-Fold method
    • LOSO
    
 # Results
 # PyTorch Results
 
![image](https://user-images.githubusercontent.com/105876342/184664947-b3731b41-7dc4-4cf1-a6f6-1abf59c224c1.png)

# TensorFlow Results
1. **For the Basketball Layer**
    
    1.1 **K-fold**



![image](https://user-images.githubusercontent.com/105876342/184665277-8ffb2123-5b3b-43e3-8d75-1730a20f08ff.png)

   
   1.2. **Leave One-Subject-Out cross-validation(LOSO) **
    
    
    
![image](https://user-images.githubusercontent.com/105876342/184665337-fa63a868-de70-45e5-b6c0-eff5bee8ae90.png)
![image](https://user-images.githubusercontent.com/105876342/184665373-49735558-ffce-47c2-8be3-80355eee129c.png)
![image](https://user-images.githubusercontent.com/105876342/184665423-a6de2b76-4aa0-43ff-a83f-4ccb80e42fd7.png)
![image](https://user-images.githubusercontent.com/105876342/184665995-2070c8d1-54ed-45f6-b477-d7aaefb6702f.png)
![image](https://user-images.githubusercontent.com/105876342/184666016-794bbfcb-0f6a-440e-8a86-c83be5e52d69.png)

    1.3. **F1 Score per class**

![image](https://user-images.githubusercontent.com/105876342/184665107-d53aa9e7-2d16-4085-994e-5eedfa2ff8ea.png)


2. **For the Locomotion Layer**

    2.1 **K-fold**

![image](https://user-images.githubusercontent.com/105876342/184666591-4d2af903-28f6-45d7-9d87-2bbe9d5fc4cc.png)

    2.2 **Leave One-Subject-Out cross-validation(LOSO)**
    
# Pre-Trained Models
You can find all the pretrained models in the folder Pre-Trained models
