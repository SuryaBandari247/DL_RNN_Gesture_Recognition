<a name="readme-top"></a>
[![LinkedIn][linkedin-shield]](https://www.linkedin.com/in/surya-bandari/)


# Deep Learning - Gesture Recognition - CNN/RNN
> A home electronics company which manufactures state of the art smart televisions. You want to develop a cool feature in the smart-TV that can recognise five different gestures performed by the user which will help users control the TV without using a remote.


## Table of Contents
* [General Information](#general-information)
* [Steps followed](#Steps)
* [Technologies Used](#technologies-used)
* [Results](#Results)
* [Acknowledgements](#acknowledgements)


## General Information
### Problem statement
> The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:

* Thumbs up:  Increase the volume
* Thumbs down: Decrease the volume
* Left swipe: 'Jump' backwards 10 seconds
* Right swipe: 'Jump' forward 10 seconds  
* Stop: Pause the movie

![image](https://github.com/SuryaBandari247/DL_RNN_Gesture_Recognition/assets/128714777/118f08e3-458a-4152-b001-d7a3f45cf829)


## Steps
We need to accomplish the following in the project:

* Generator:  The generator should be able to take a batch of videos as input without any error. Steps like cropping, resizing and normalization should be performed successfully.

* Model: Develop a model that is able to train without any errors which will be judged on the total number of parameters (as the inference(prediction) time should be less) and the accuracy achieved. As suggested by Snehansu, start training on a small amount of data and then proceed further.

Thus, there are two types of architecture commonly used for analysing videos, both explained below. 

**Convolutions + RNN**
The conv2D network will extract a feature vector for each image, and a sequence of these feature vectors is then fed to an RNN-based network. The output of the RNN is a regular softmax (for a classification problem such as this one). 

**3D Convolutional Network, or Conv3D**
3D convolutions are a natural extension to the 2D convolutions you are already familiar with. Just like in 2D conv, you move the filter in two directions (x and y), in 3D conv, you move the filter in three directions (x, y and z). In this case, the input to a 3D conv is a video (which is a sequence of 30 RGB images). If we assume that the shape of each image is 100x100x3, for example, the video becomes a 4-D tensor of shape 100x100x3x30 which can be written as (100x100x30)x3 where 3 is the number of channels. Hence, deriving the analogy from 2-D convolutions where a 2-D kernel/filter (a square filter) is represented as (fxf)xc where f is filter size and c is the number of channels, a 3-D kernel/filter (a 'cubic' filter) is represented as (fxfxf)xc (here c = 3 since the input images have three channels). This cubic filter will now '3D-convolve' on each of the three channels of the (100x100x30) tensor.

## Technologies Used
- Jupyter notebook - version 6.4.12
- Python - version 3.10.0
- Pandas - version 2.0
- Numpy - version 1.24.2
- sklearn - version - 1.2.2
- seaborn - version - 0.12.2
- Tesnorflow
- Keras API


## Results

![image](https://github.com/SuryaBandari247/DL_RNN_Gesture_Recognition/assets/128714777/0405d815-97ca-4734-9930-76a631f05d1c)



 

## Acknowledgements
- Upgrad
- Google in general

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
## Contact
Created by [@suryabandari247](https://www.linkedin.com/in/surya-bandari/) - feel free to contact me!
