# NASSMA 2019: ConvNets and Computer Vision Tutorial
*Adapted from a tutorial by Viorica Patraucean.*

## Focus of the tutorial: Build a convolutional neural networks for image classification, plus some more advanced concepts as a bonus.

#### Part I (baseline.ipynb): Training a baseline convnet classifier
* build a simple classifier given a specific architecture structure
* get dataset, apply data augmentation (cropping, flipping)
* train classifier
* check number of parameters

#### Optional: Part II (distillation.ipynb): [Distilling the knowledge](https://arxiv.org/pdf/1503.02531.pdf) from a (larger) teacher model
* import an already trained baseline model to use as teacher
* use the smaller baseline model as student
* add KL distillation loss between teacher and student
* train the student classifier with this joint loss

#### Bonus (visualisation.ipynb): Visualise saliency maps (e.g. [paper](https://arxiv.org/pdf/1312.6034v2.pdf))
* import an already trained model
* visualise the gradients of class probabilities w.r.t inputs to obtain saliency maps
* visualise inputs that maximize class probabilities

## Conclusion
* Convolutional models achieve high accuracy in image classification.
* Distillation is a simple technique for training smaller models to achieve accuracy similar to larger models. It can be used on its own or in conjunction with techniques like separable convolutions.
* Backpropagation is used for training neural networks, but can also be used to visualise what a network has learnt.
* Although these models are very good, there are still important open research questions about how to make them more robust to various attacks.
