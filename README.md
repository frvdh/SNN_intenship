# SNN_internship

Results of Spiking neural networks internship done at IMEC Leuven during Summer of 2021 with the neuromorphic radar team
---
My internship at [IMEC](https://www.imec-int.com/en) started in the beginning of July 2021 with learning the main theoretical concepts and practices used in the current deep learning and SNN field. The programming language and main library used for this were Python and Pytorch. Using some sample code that trains and tests a vanilla SNN, following animation was generated:

https://user-images.githubusercontent.com/47596729/127158387-fa131bec-445b-4f30-bbcf-011ec641bcae.mp4

The left images are some MNIST-images taken from a batch with size 200 and the prediction of the network can be seen above the right images.

To understand the right-hand image, the input of the net should first be explained. A batch contains 200 images and the net takes as input a tensor with dimensions (200,i,28). This tensor contains the 28 pixel values of the i-th row of the 200 batch images. This input goes through a first layer and subsequently through the net's only hidden layer with 150 neurons which outputs a (28,200,150) tensor. This tensor is then showed in a page-per-page (e.g. page 1 is (1, 200, 150)) manner in the video to show the neuron activity of the hidden neurons in the network.

The net's test accuracy is 95.98%.
