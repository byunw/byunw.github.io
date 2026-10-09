---
permalink: /projects/
layout: single
author_profile: false
---

Project Link

https://colab.research.google.com/drive/1Y0QKG7ma0KMVf9qXPS2w6HZqUVz8HEww?authuser=2#scrollTo=3758d381

My GoogleColab consists of 4 cells. Let's talk about what each cell does in this section.
The code in the first cell copies 3 files and a folder to /content.
Similar to the first cell, the second cell does not have much code. The second cell only has the following code: !nvidia-smi.
By running the code, I can know which device was assigned. In my case, a NVIDIA A100-SXM4-80GB was assigned. 
I do not yet know the internal of NVIDIA A100-SXM4-80GB. 

Before the training happens, the training dataset is loaded onto the ram (not onto the GPU).
Since the GPU will be used, the value of device.type will be "cuda" (device.type value gets stored on the ram). 3047,1044 parameters are first loaded onto the ram and they are copied to the GPU. The learning rate is initially 3e-5 and the epoch is 20. epoch and learning rate are called hyperparameters. 

The loss is calculated for each epoch. Before the forward pass happens, the current batch of 1-lead ecgs are loaded onto the ram
and are copied to the GPU. The corresponding labels are also loaded onto the ram and are copied to the GPU. Now, Let's dive into the internal
of Hubert-ECG. The first layer of Hubert-ECG is the convolution layer and this convolution layer converts 1-lead ecg (a vector of size 9,000) into a matrix of size 512x2248.  














