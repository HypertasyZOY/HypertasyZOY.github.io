---
layout: post
title:  "Thinking about hyperparameters"
date:   2018-03-20
categories: MachineLearning Thinking
tags: [Dark Hyperparameters, Neural Network]
---
Today, I am tuning my two layers neural network. In CS231n assignment 1. 
##What are we actually tuning.
##### Learning rate & Learning rate decay

##### Regulations & drop out possibility
Regulations can limit the difference between train_acc and val_acc. It has limited influence towards test_acc since regulation itself is trained and selected by val_set. So does drop out. But regulation will restrict the express ability of model. Strong regulation sets a lower upper limit for models.
Drop-out divides the total Neural Network into several mixed modules. During the training process, for example, pictures in the car category are trained by different neurons combinations. Each of these combinations may also trained by other pictures, no matter about the pictures' categories. When testing, these model combinations fight, yield, and vote for outcomes. If the car model combinations are yelling louder than other models' combinations, the outcome is class car. During the car recognition train process, a sub-process within the whole training, the selected model combinations are trained to speak louder on class car. Therefore, during the testing process, these car model combinations will shout louder than those model combinations which are not trained by car pictures, since they are more likely to speak in normal way as they are not optimized to speak loud when meeting cars.
##### hidden layers' amounts and sizes
##A tip for saving time



