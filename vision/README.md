# NASSMA 2019: ConvNets and Computer Vision Tutorial
*Adapted from a tutorial by Viorica Patraucean.*

## Focus of the tutorial: Study on the efficiency and robustness of convolutional neural networks for image classification

#### Part I (baseline.ipynb): Training a baseline convnet classifier
* build a simple classifier given a specific architecture structure
* get dataset, apply data augmentation (cropping, flipping)
* train classifier
* check number of parameters

#### Part II (visualisation.ipynb): Visualise saliency maps (e.g. [paper](https://arxiv.org/pdf/1312.6034v2.pdf))
* import an already trained model
* visualise the gradients of class probabilities w.r.t inputs to obtain saliency maps
* visualise inputs that maximize class probabilities

#### Part III (distillation.ipynb): [Distilling the knowledge](https://arxiv.org/pdf/1503.02531.pdf) from a (larger) teacher model
* import an already trained baseline model to use as teacher
* use the smaller baseline model as student
* add KL distillation loss between teacher and student
* train the student classifier with this joint loss

#### Part IV (optional): Test robusness of models using simple geometric transformations
* several recent papers have shown that convnets are not robust to simple geometric transformations, e.g. [paper1](https://arxiv.org/pdf/1805.12177.pdf), [paper2](https://arxiv.org/pdf/1711.09115.pdf)
* starting for example from the visualisation colab in part II, write a function that: (1) slides crops over Cifar test set images
(2) feeds the crops into the pre-trained baseline model; (3) plots predictions per class per crop. Are they stable?

## Conclusion
* Convolutional models achieve high accuracy in image classification.
* Backpropagation is used for training neural networks, but can also be used to visualise what a network has learnt.
* Distillation is a simple technique for training smaller models to achieve accuracy similar to larger models. It can be used on its own or in conjunction with techniques like separable convolutions.
* Although these models are very good, there are still important open research questions about how to make them more robust to various attacks.
