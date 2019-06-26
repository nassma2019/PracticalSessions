# Hello, NASSMA!
adapted from TMLSS 2018 lab by David Szepesvari

_Designed for education purposes. Please do not distribute without permission_. 

This colaboratory (colab) will help you get prepared for the rest of the practical sessions at NASSMA.

Here you will get familiar with the environment and tools used in the rest of the practical sessions. **We strongly encourage you to go through these tutorials before the school**. There are small exercises throughout the sections to help you internalize the topics covered and to check your understanding. Finally, there is also a comprehensive exercise where you use all these tools to train an mnist digit classifier. **The other lab sessions will assume you can do this**.

The introductory lab session itself will be used to clarify any questions.

_Special thanks to the authors of educational material at DeepMind, as their work was a great resource for the creation of this lab_.

## Lab 1.1: What is colab?
This colab teaches you about colab and its main features. You will need to know this for the rest of the labs as you will write all code in colab.

Open the file _Intro: Colab.ipynb_ to access the colab.

## Lab 1.2: Introduction to Numpy and matplotlib.
This colab introduces you to numpy, the python package we use for computing and linear algebra. Topics such as

* array creation
* operations on arrays
* indexing and selection on arrays
are covered.

We will also cover how to plot data using Matplotlib:


* draw line plots so we can visualize training curves later, and
* display images, or galleries of images so we can visualize the inputs/outputs of vision models.

By the end of this colab you will know how to make plots in Python, and will have written a function to generate datasets for learning the NXOR function (used in the rest of the lab).

Open the file _Intro: Numpy And Plotting.ipynb_ to access the colab.

## Lab 1.3: Training an NXOR classifier with Tensorflow and Sonnet
In this colab you learn how to build tf and [sonnet](https://github.com/deepmind/sonnet) models that will be useful in the computer vision and NLP lab. We also cover topics like

* a number of lower level tensor operations
* visualizing the model we built
* getting the data into our model
* debugging tensorflow models
* backpropagation as implemented by tensorflow
* how to actually train the network.
By the end of the colab you will have trained a classifier that approximates the NXOR function.

Open the file _Intro_Tensorflow_and_Sonnet.ipynb_ to access the colab.

## Exercise: putting everything together
In this colab you will write code for a model that learns to classify mnist digits. You will use sonnet and tensorflow, tracking training progress with matplotlib.

Colabs:

* Exercise: _Comprehensive Exercise.ipynb_
* Solutions: _Comprehensive Exercise [Solution].ipynb_
