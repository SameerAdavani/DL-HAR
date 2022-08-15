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
Models using Pytorch. All the models were trained using the 80:20 approach only. The models are as follows:

    • Single LSTM Model 
    • Double Stacked LSTM Model
    • ResNet (Transfer learning model) 

Using TensorFlow, we used only 1 model but we had three approaches. The model is similar to the Single LSTM model. The TensorFlow model was used for the Basketball layer and Locomotion Layer. The three approaches for the model are:
    
    • 80:20 Split
    • K-Fold method
    • LOSO
    
 # Results
 # PyTorch Results
 Class Training(Drill) % Validation(Drill) % Testing(Game) %
Dribbling 99.8 97.6 43
Shot 99.8 97.1 27
Pass 98.8 65.8 25
Layup 99.76 90.3 25
Rebound 99.76 21.9 4
Table 6: F1 Score per class for Single LSTM mode


