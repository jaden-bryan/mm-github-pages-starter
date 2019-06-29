---
permalink: /ocean-institute/
title: "Neural networks in marine biology applications"
---

A neural network is a group of algorithms modeled after the human brain trained to recognize patterns.  My research this year focused on applying neural networks to the identification of various organisms off of California’s coast.  The almost infinite biodiversity of the ocean means that even the most experienced marine biologists have to turn to resources and guides when the occasional, unknown organism appears.  This books and databases of marine life are extremely dense making identification a very time-consuming process.  The goal of my research is to begin to create an application that can take an image of an unidentified organism and instantaneously determine what is being depicted in the camera input. 
 
Having worked with neural networks before, I was fairly confident that such programs could find success in my research .  The first step in making a neural network is getting an abundant supply of image data.  I would video each organism that I wanted my application to be able to identify for approximately 30 seconds, then would split the video into thousands of images using FFMPEG.  These images were then converted into a dataflow graph by an application called TensorFlow.  

To simplify the process of creating an image classifier, I based my model on the existing image network, Inception V3 (see image directly below).  This network already contains useful information classifying abilities that are universally applicable to image data.  I simply trained the final ‘layer’ of this network in order to specifically target marine animals as input.  

The application was able to identify organisms using image data with an accuracy of 95-99%, meaning high confidence in each prediction.  Furthermore, I was able to successfully port the network to both mobile and desktop platforms, increasing its usefulness and versatility.  

On an Android device, the network is able to identify organisms successfully using live camera input.  On iOS and desktop, static images must be used, but I am currently working on implementing live feeds to both of these platforms as well.

The more image data provided during the training process, the more accurate the classifier became.  Additionally, allowing for the network to ‘train’ for longer by removing the limit for iterations done for each image set allowed for the application to increase its confidence percentage to an even greater degree.

Neural Networks can effectively be used to identify marine organisms using image data.  

If you have any questions about this project please send me an email using the address below.  

jdn.bry@gmail.com
