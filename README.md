# American Sign Language (ASL) Translator

A machine learning model utilized to predict letters and numbers from the American Sign Language alphabet in real time.

## Overview

This project was originally developed during [HackWesTX2020](https://www.hackwestx.tech/). The idea was to bridge the gap between English speakers and deaf/nonverbal people. To do so, the convolutional neural network is trained on a dataset from Kaggle titled [_ASL-dataset_ by ayuraj](https://www.kaggle.com/datasets/ayuraj/asl-dataset). 

## Models

The machine learning model developed is a simple convolutional neural network instantiated as a sequential model. It consists of 6 layers total. 

The first layer is a convolutional 2D layer with 32 filters and a 5x5 kernel shape. This is followed by an average pooling 2D layer. The next two layers are essentially the same but with 64 filters. Next, the layers are flattened. For the last two layers, dense layers are used. The first one has 128 units (shape of the image) and the second one has 36 units (number of classes). Each of these layers use a ReLU activation function except for the last dense layer which utilizes softmax.

The model is then compiled with adam optimizer and categorical cross entropy for its loss function. The accuracy, precision, and recall are set as the metrics. 

## Evaluation

Overall, the model achieved a 95.6% accuracy, 95% precision, and 95.6% recall.
![image](https://github.com/Jeremy-Vidaurri/ASL-Translator/assets/10247339/8b79d308-f718-4279-af56-11bfd81cd019)

![image](https://github.com/Jeremy-Vidaurri/ASL-Translator/assets/10247339/80952ae5-21ce-4026-82e0-b0436fb1dba7)



