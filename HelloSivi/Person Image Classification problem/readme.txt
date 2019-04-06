
 File Description:

 1. keras_multiclass_person_or_not.ipynb -jupyter notebook containing alogorithm and approach
 2. keras_multiclass_person_or_not.py - same file in python file format containing algorithm and approach
 3. person-model.h5 and person-model.json - pretrained models which can be loaded and used for prediction
    person or not
 4. model accuracy verifier.ipynb - consists of code on to how load pretrained models and verify the accuracy
    if there is any premapped prediction.

Dataset Description and Approach

This is self created dataset which a combination of 2 datasets person dataset from internet and cat-dog datasets
from machine hack website.

I have trained my model human images in case to identify persons
and trained cats and dogs to be identified as non-person

 - test data contains 60 images
 - trained data contains 827 images
 - prediction data contains 10 images

 Model explanation

 - I have used Convolutional Neural Network to solve this problem statement
 - 3 Convolutional layers
 - then a flatten layer
 - continued by 2 Dense layers and a output layer
 - dropout has been used in dense layers to avoid overfitting

 Model verifier

 - easily verify the model using the verifier code
