# Mask_Detection_project
## Overview
It is rightly said that "Necessity is the mother of all inventions".We all know that for the past 2 years the world has been in a jeopardize due to COVID-19 pandemic. We still do not have proper medicines for COVID-19 and our only protection against this disease is vaccination and precaution. In these tough times, technology has again come to aid humanity with unique and innovative solutions. One of these is the COVID-19 face mask detection system using machine learning.
Being a budding engineer and machine learning enthusiast, I tried to implement one of these face mask detection systems as a part of my college project. This face mask detection system uses concept of transfer learning to classify face images taken from live video stream into two categories, <b>with_mask</b> and <b>without_mask</b>. By using transfer learning, I have tried to save a huge amount of time which usually gets invested in training deep neural networks. 
In my project I am using Google’s state of the art CNN architecture- MobileNetV2, which is a very light weight CNN architecture that allows it to be used even with limited computational powers of mobile phones. If deployed correctly, the COVID-19 mask detector I built could potentially be used to help ensure your safety and the safety of others.

## About transfer learning
In transfer learning, the knowledge of an already trained machine learning model is applied to a different but related problem. For example, if you trained a simple classifier to predict whether an image contains a backpack, you could use the knowledge that the model gained during its training to recognize other objects like sunglasses.
The general idea is to use the knowledge a model has learned from a task with a lot of available labeled training data in a new task that doesn't have much data. Instead of starting the learning process from scratch, we start with patterns learned from solving a related task.

![image](https://user-images.githubusercontent.com/52367430/142389599-75f61d8f-2be9-481f-8a66-319810c1f29c.png)

In computer vision, for example, neural networks usually try to detect edges in the earlier layers, shapes in the middle layer and some task-specific features in the later layers. In transfer learning, the early and middle layers are used and we only retrain the latter layers. It helps leverage the labeled data of the task it was initially trained on. We try to transfer as much knowledge as possible from the previous task the model was trained on to the new task at hand. This knowledge can be in various forms depending on the problem and the data.
Transfer learning has several benefits, but the main advantages are saving training time, better performance of neural networks (in most cases), and not needing a lot of data. Usually, a lot of data is needed to train a neural network from scratch but access to that data isn't always available — this is where transfer learning comes in handy. With transfer learning a solid machine learning model can be built with comparatively little training data because the model is already pre-trained.

## Dataset
The data set consists of 1,376 images in total, belonging to two classes.
•	With_mask: 690 images
•	Without_mask: 686 images

## Pipeline

![image](https://user-images.githubusercontent.com/52367430/142391579-f69ec0a7-0c90-4b73-afb4-aa1e96194e99.png)

## Performance

![image](https://user-images.githubusercontent.com/52367430/142391747-7cc5aa15-6ba9-43c9-b798-1c390af88936.png)

classification report on test-set:

![image](https://user-images.githubusercontent.com/52367430/142391915-37108f07-65ae-428e-8378-ebd1706530e8.png)

## Results

https://user-images.githubusercontent.com/52367430/142372645-c181753f-e8db-4328-a065-2cd8bc0a5d62.mp4
