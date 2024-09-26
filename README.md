# Project Overview

This project aimed to train a custom Deep Convolutional Neural Network to detect forest fire smoke in video footage. The dataset used to train the model comes from the [HPWREN Fire Ignition Library](https://www.hpwren.ucsd.edu/FIgLib/) - a library that focuses primarily on California forest fires. 

This project utilized the VGG16 model architecture for the backbone of the model and feature extraction. The output of the CNN is passed to a fully connected layer where the model then bifurcates (into 2 ouptuts). One output is for regression, as it is predicting the coordinates of the bounding box. Meanwhile, the other output is for classification prediction. 

The model was trained on a dataset of images sourced from time-lapse recordings of forest fires in their early stages. Once trained, the model can also be applied to video footage by making predictions on indivdual frames. 

Here are two examples of the model being applied to video footage:

https://github.com/user-attachments/assets/db79a343-9d31-4751-b1b4-ef99683e34bc

https://github.com/user-attachments/assets/b255fe5c-dbd5-4610-af37-dfd6b7671134
