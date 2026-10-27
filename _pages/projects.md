---
permalink: /projects/
layout: single
author_profile: false
---


Contributor: Woosuk Byun (변우석)

Advisor: Professor Haibo Yang

Problem Statement: Classifying single-lead ECG recordings into four classes: Normal (N), Atrial Fibrillation (A), Other Rhythm (O), and Noisy (~). 


Dataset: The original dataset had 8,528 1-lead ECGs and their truth labels (N,A,O,~). 
The dataset can be downloaded from the following: [Click Here](https://physionet.org/content/challenge-2017/1.0.0/).
There are 5,050 1-lead ECGs which are labeled as N. There are 2,456 1-lead ECGs which are labeled as O. There are 738 1-lead ECGs which are labeled as A. There are 284 1-lead ECGs which are labeled as ~. The majority of the 1-lead ECGs are labeled as N. In other words, the dataset is imbalanced. How was the whole dataset split into the training dataset, the validation set and the test dataset? The training dataset is approximately 70% of the original dataset (5,969 samples). The validation dataset is approximately 15% of the original dataset (1,279 data samples). The test dataset is approximately 15% of the original dataset (1,280 samples). The training dataset has approximately the same distribution of N,A,O,~ as that of the original dataset. The validation dataset has approximately the same distribution of N,A,O,~ as that of the original dataset. The test dataset has approximately the same distribution of N,A,O,~ as that of the original dataset. 


Data Preprocessing: Out of all the training 1-lead ECGs, 4163 1-lead ecgs have a length of 9,000, 
                    1,107 1-lead ecgs have a length longer than 9,000. 699 1-lead ecgs have a length shorter than 9,000.
                    
Training:

My GoogleColab consists of 4 cells. Let's talk about what each cell does in this section.
The code in the first cell copies 3 files and a folder to /content.
Similar to the first cell, the second cell does not have much code. The second cell only has the following code: !nvidia-smi.
By running the code, I can know which device was assigned. In my case, a NVIDIA A100-SXM4-80GB was assigned. 
I do not yet know the internal of NVIDIA A100-SXM4-80GB. 

Before the training happens, the training dataset is loaded onto the ram (not onto the GPU).
Since the GPU will be used, the value of device.type will be "cuda" (device.type value gets stored on the ram). 3047,1044 parameters are first loaded onto the ram and they are copied to the GPU. The learning rate is initially 3e-5 and the epoch is 20. epoch and learning rate are called hyperparameters. 

The loss is calculated for each epoch. Before the forward pass happens, the current batch of 1-lead ecgs are loaded onto the ram
and are copied to the GPU. The corresponding labels are also loaded onto the ram and are copied to the GPU. Now, Let's dive into the internal
of Hubert-ECG. The first layer of Hubert-ECG is the convolution layer and this convolution layer converts 1-lead ecg (a vector of size 9,000) into a matrix of size 512x2248. The next layer is GELUActivation layer and this layer's output has the same dimension as before 512x2248. The next layer (GroupNormalization) preserves the same dimension as before 512x2248. The output of the GroupNormalization layer is fed into the convolutional layer and the output of the convolution layer is 512x1123.
This 512x1123 matrix is fed into the GeluActivation layer whose output has the dimension of 512x1123 and this output is again fed into the conv layer and the conv layer produces a matrix of 512x1123. The second GeluActivation layer produces a matrix of 512x1123 and the third conv layer produces a matrix of 512x561 and the output of the third convolutional layer is fed into the third GeluActivation layer and this GeluActivation layer produces a matrix of 512x561 and the next conv layer produces a matrix of 512x280 and the next GeluActivation layer produces a matrix of 512x280. Then the LayerNormalization layer produces a matrix of 512x280 and each column of this matrix is fed into the fully-connected neural network which produces a vector of 512 elements, resulting in a matrix of 512x280. And this matrix stays the same even after the Dropout. The matrix after the Dropout layer will result in a matrix of 512x281 after the convolutional layer and the HubertSamePadLayer truncates the last column, resulting in a matrix of 512x280 and GeluActivation layer is applied on the 512x280 matrix, resulting in a matrix of 512x280. 

To be written more soon. 

Evaluation: To be written soon.

Model Deployment: To be written soon.













