# **Image-Based Deep Learning: *Finding Pneumonia in Labeled Optical Coherence Tomography (OCT) and Chest X-Ray Images***

Analysis by Jonny Hofmeister for Flatiron School Phase 4 Project

This X-ray image data comes from [the Mendeley Website and contributors from UCSD.](https://data.mendeley.com/datasets/rscbjbr9sj/3)

## **Pneumonia in X-Rays**

While blood and sputum tests are used to confim pneumonia infections, chest X-rays of the lungs have long been used by doctors to help diagnose and determine the extent and location of the infection. 

*Can we use this labeled x-ray image data to train a machine learning model to recognize the infections?*
  - Assistance from models could help busy medical staff diagnose routine infections faster and smoother.
  - Also could help diagnose infections with a higher level of certainty - who wouldn't want their result confirmed by more that one source?

<img src="images/jZqpV51.png">

## **The Data**

This dataset, from University of California San Diego, Guangzhou Women and Children's Medical Center, contains 5840 labeled X-ray images. The images vary significantly in size and will be scaled down for input into the model. Visually based on the images, patients vary in age from babies to adults; but no other information is provided with the data besides the image file and class label - NORMAL or PNEUMONIA.

## **Modeling**

***Why a Nerual Network?***

Neural Networks and Deep Learning tools are currently the best we have at our dispoal for processing and learning patterns in image data. Tensorflow and Keras will be the deep learning packages used for this project.

I will create 2 models:
  1. A simple baseline network
      - A simple model with only a few hidden layers will show us the potential of the data without taking too much processing time.
  
  2. Convolutional Neural Network
      - Convolution is a common image processing technique that allows us to extract more localized patterns in 2D images
      - CNNs are very successful at tasks like this, and tuning one will likely produce our best results.

## **Results**
