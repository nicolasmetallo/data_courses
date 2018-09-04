# Machine Learning for Urban Cities
## Final Project Report
![N|Solid](http://magnet.nyu.edu/wp-content/uploads/2015/10/CUSP_logo.jpg)

**Professor:** Gustavo Nonato

**Team:** Nicolas Metallo, Niraj Nagarajan

**Date:** May 8, 2017

This is the support documentation for our ML final project where we present a simple example for using computer vision to empower people with blindness and low vision to do more.

## What's the problem?
Thanks to a lawsuit brought by the American Council of the Blind (ACB), the Treasury Department must make US currency accessible to blind and visually impaired Americans under the Rehabilitation Act of 1973. Unfortunately, the wheels of government grind slowly, and banknotes with braille identification won't be in circulation until 2020. Some devices and smartphone apps already exist in the market that do a simple banknote identification, but we wanted to create a novel and customizable solution using machine learning that would set the foundations for solutions that can easily extend these capabilities to other currencies.

## What's our solution?
Use transfer learning with a pretrained GoogLeNet neural net to re-train the last layer and create a new image classification algorithm than can accurately identify US dollar banknotes. 

## Description
We are using a dataset of 4000 photos separated into four different classes: 1 dollar, 5 dollars, 10 dollars and 20 dollars. We split our data into 60% training data, 25% test data and 15% validation data.
We then use both Tensorflow and Caffe (through NVIDIA DIGITS) to train our model and measure its accuracy. In the end, the Caffe model was more accurate with up to 92.5% accuracy in our validation tests.

## What's the tech behind it?

We used different open source resources to create our project:

* Python
* Amazon AWS (p2.large)
* Docker
* Tensorflow
* Caffe
* NVIDIA Dockers
* NVIDIA GPU REST Engine
* NVIDIA DIGITS 5
* Tesseract
* Raspberry Pi

## Files in this Repository
- Use Tesseract OCR engine as a Web API
- Image Recognition Using GPUs in Amazon ECS Docker Containers
- Image Caption Generation as a Web API