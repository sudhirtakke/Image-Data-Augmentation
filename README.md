# Image-Data-Augmentation
IMAGE AUGMENTATION WHILE TRAINING DEEP LEARNING NEURAL NETWORKS

A technique that can be used to artificially expand the size of training dataset by creating modified versions of images in the dataset.

Training deep learning neural network models on more data can result in more skillful models, and the augmnetation techniques can create variations of the images that can improve the ability of the fit models to generalize what they have learned to new images.

The Keras deep learning neural network library provides the capability to fit models using image data augmentation via the ImageDataGenerator class.


Image data augmentation is used to expand the training dataset in order to improve the performance and ability of the model to generalize.
Image data augmnetation is supported in the Keras deep learning library via the ImageDataGenerator class.
How to use shift, flip, brightness, and zoom image data augmentation

### Intent of Image Augmentation

Expand the training dataset with new, plausible examples. This means, variations of the training set images that are likely to be seen by the model. For example:

A horizontal flip of a picture of a cat may make sense, because the photo could have been taken from the left or right.
A vertical flip of the photo of a cat does not make sense and would probably not be appropriate given that the model is very unlikely to see a photo of an upside down cat.

It is clear that the choice of the specific data augmentation techniques used for a training datset must be chose carefully and within the context of the training dataset and knowledge of the problem domain.
It can be useful in experiment with data augmentation methods in isolation and in concern to see if they result in a measurable improvement to model performance perhaps with a small prototype dataset, model, and training run

Modern deep learning algorithms, such as CNN can learn features that are invariant to their location in the image.
Augmeantation can further aid in this transform invariant approach to learning and can aid the model in learning features that are also invariant to transform such as left-to-right to top-to-bottom ordering, light levels in photographs, and more.

Image data augmentation is typically only applied to the training dataset, and not to the validation or test dataset. This is different from data preparation such as image resizing and pixel scaling; they must be performed consistently across all datasets that interact with the model

[Jupyter Notebook](./Data_augmentation.ipynb)
