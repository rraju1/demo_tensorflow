# Tensorflow script for Camera demo

This script serves as a example to creating a neural network model in Tensorflow which is meant to be deployed on a DE1-SoC FPGA. This model will obviously have to be quantized to lower 8-bit representation in addition to the activations. This will most likely be done with the Graph Transform Tool provided by Tensorflow.

The task we are interested in solving is classifying different kinds of street signs. Our toy example will be looking at 4 different kinds of signs. The input to the network is a 120x160 image from the TRDB-D5M camera which will be feed into a five-layer network, with 4 convolutional layers and one full-connected layer. 
