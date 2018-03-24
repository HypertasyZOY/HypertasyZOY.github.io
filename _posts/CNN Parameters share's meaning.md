 ---
layout: post
title:  "CNN Parameters share's meaning"
date:   2018-03-23
categories: MachineLearning DeepLearning Thinking
tags: [Neural Network, CNN]
---
It actually solves this problem when extending a trained network to universe:
How to figure figure out a feature when this feature appears in different locations of various pictures.

Since each slice of the first corresponds to a filter for only one feature, the more slices, the better.
And since the following layer will take this layer's output as input, namely taking fixed features in different locations as input, the number of features filters must be enough for following layers

![Kri CNN's weights](media/15218007800863/Kri%20CNN's%20weights.jpeg)


