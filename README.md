# Project on Computer Vision Mask Detection

## Overview
### What is computer vision?

Computer vision is part of Artificial Intelligence, which enables computers to mimic the human brain and teach computers to learn from the given input.  


## Objective
Today I am going to present how computer vision is used to detect a human face


with mask

<img src="https://user-images.githubusercontent.com/100771366/171874826-c214dea9-c1c0-435f-a01e-ca8cda3d0246.png" width="114" height="114" />


or without mask

![437](https://user-images.githubusercontent.com/100771366/171874875-c5dfd7d2-7031-4680-b16d-89db53638894.png)

### Import Libraries

<img src="https://user-images.githubusercontent.com/100771366/171991985-6f9a197c-1bb2-4e10-8858-3052cc673305.png" width="800" height="200" />

### Import Dataset

Import dataset using ImageDataGenerator and set the parameters

### Use pre trained model - Sequential Convolutional Neural Network 
Convolutional neural network models are good in image recognition.<br/>
They have strong ability in abstracting spatial information from multiple levels<br/>
Convolutional connections help to reduce the computational cost, number of parameters, and overfitting risk<br/>
In SCNN multilayered neural networks stacked and hidden layers are formed on top of each other in a sequence<br/>
This helps the convolutional neural networks  to learn the hierarchical features

<img src="https://user-images.githubusercontent.com/100771366/171991989-15f8d99f-1feb-48c0-8285-4764556a9ae2.png" width="800" height="200" />

### Compile the model
Using Adam optimizer,<br/>
Binary crossentropy loss function,<br/>
and matrics = accuracy 

### Fit the model 
history = model.fit(train_generator, epochs = epoch, validation_data = valid_generator,batch_size = batch_size )<br/>
The accuracy achieved on training dataset and validation dataset is almost **98%**

### Training loss and Validation loss
The loss closer to zero better the model perfomance

<img src="https://user-images.githubusercontent.com/100771366/171991991-2ee54127-a63f-4f6e-9a1e-55da10e1292b.png" width="800" height="400" />

### Model's Mask Detection 
<img src="https://user-images.githubusercontent.com/100771366/171991993-ea6f5672-9ed0-481b-9167-72d38e5f5c8b.png" width="114" height="600" />
<img src="https://user-images.githubusercontent.com/100771366/171991996-6a647e4c-cb50-494a-b922-87909036ca74.png" width="114" height="600" />

### But some of the pictures were not detected correctly
<img src="https://user-images.githubusercontent.com/100771366/171991997-db714b41-1334-4b81-86c6-344b9893facb.png" width="114" height="600" />
<img src="https://user-images.githubusercontent.com/100771366/171991999-f25c83dd-f6a6-4819-925f-2d3eddf5220d.png" width="114" height="600" />

## Thank You 




