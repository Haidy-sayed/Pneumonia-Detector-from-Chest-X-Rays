\# 🫁 Pneumonia Detection from Chest X-Rays



\## Overview

A neural network classifier built from scratch 

to detect pneumonia from chest X-ray images.



\## Motivation

As a biomedical engineer moving into Medical AI, this project 

bridges my clinical domain knowledge with deep learning.



\## What I Applied

\- Neural network architecture (forward/backward propagation)

\- Batch normalization

\- Dropout regularization

\- Adam optimizer

\- Bias/variance diagnosis via learning curves

\- He weight initialization



\## Results till 16-06-2026

\[Test accuracy 71.79%] >>> will tune the parametrs later (I think i should increase the hidden layers size cuz now we are running on jst 2 layers 1 hidden and 1 output)
\[Test accuracy 73.40%] >>> after increasing the number of epochs to 100.       Dated : 10.28.26



\## Dataset

Kaggle Chest X-Ray Images (Pneumonia) — 5,863 images



I balanced for the training set Both the normal and Pneumonia to be 1330 images , added more mages to the val and test sets for both as well to avoid overfitiing 



dataset url : https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia?resource=download




Dataset Manipulation and Final Distribution
The original dataset was reorganized to address class imbalance in training and to establish a larger validation set for model selection and a separate test set for final evaluation. Images were reassigned from the original training set to the validation and test sets; no new images were introduced.
The training set was balanced to contain 1,330 images per class. The final dataset distribution is as follows:
Split
Normal
Pneumonia
Total
Training
1,330
1,330
2,660
Validation
30
48
78
Testing
234
300
534
Total
1,594
1,678
3,272

Training-set balancing: The original training set contained approximately 2.89 pneumonia images for every normal image, with pneumonia representing approximately 74.3% of the training data. To address this imbalance, the training set was balanced to a 1:1 class ratio. The resulting training set contains 2,660 images, with 1,330 images in each class.


Validation-set modification: The validation set was increased from 16 to 78 images by reallocating images from the original training set. This provides more evaluation examples for model selection and hyperparameter tuning, although the resulting set remains relatively small.


Test-set modification: The test set contains 534 images, including 234 normal images and 300 pneumonia images. The original test set was reduced from 624 images to 534 images. The test set is reserved for final performance evaluation and is not used for model training or model selection.


The final dataset contains 3,272 images across training, validation, and testing. All reported performance metrics will be calculated using the designated evaluation sets, with the test set remaining untouched until the final model evaluation.


Manipulated Data Set URL "https://drive.google.com/drive/folders/1IAGEJF_xJeVSPK_Q5ADtZvDDgZBTFS02?usp=sharing"
\## How to Run

Just run the notebook pneumonia\_detector.ipynb , each cell successively 

