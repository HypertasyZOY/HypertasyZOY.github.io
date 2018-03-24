 ---
layout: post
title:  "CNN Parameters share's meaning"
date:   2018-03-23
categories: MachineLearning DeepLearning Thinking
tags: [Neural Network, CNN]
---
Default cited from http://cs231n.github.io/convolutional-networks/

It actually solves this problem when extending a trained network to universe:
How to figure figure out a feature when this feature appears in different locations of various pictures.

Since each slice of the first corresponds to a filter for only one feature, the more slices, the better.
And since the following layer will take this layer's output as input, namely taking fixed features in different locations as input, the number of features filters must be enough for following layers

However:
" One practical example is when the input are faces that have been centered in the image. You might expect that different eye-specific or hair-specific features could (and should) be learned in different spatial locations. In that case it is common to relax the parameter sharing scheme, and instead simply call the layer a Locally-Connected Layer."

![Kri CNN's weights](/img/Kri%20CNN's%20weights.jpeg)

"Example filters learned by Krizhevsky et al. Each of the 96 filters shown here is of size [11x11x3], and each one is shared by the 55*55 neurons in one depth slice."
