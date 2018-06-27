# PR061
Ophthalmological Diagnosis System  Based on Deep Learning
========
Design Introduction
------
The diagnosis system of Ophthalmology based on deep learning uses a convolutional neural network on the basis of Intel OpenCL FPGA hardware acceleration as the forward operation framework. We have done the system on De10-Nano development board. It combines the high quality picture samples of congenital cataract with Caffe to trains the AlexNet deep learning model and replaces the trained weight files to the convolutional neural network. The eye samples were collected through the camera and sent into the neural network to make binary classification results. Finally, a system with congenital cataract diagnosis function was established.
This project is mainly done in OpenCL and C++, where all the kernels are written in OpenCL and host code running on the ARM in C++. The Altera OpenCL SDK allows a programmer to use high level code to generate an FPGA design with low-power consumption and good performance. Alrera’s AOCL compiler is used to compile the Kernel code to FPGA design and automatically generates System Verilog code for the developer.
By using the convolution neural network based on Intel OpenCL FPGA hardware acceleration, we can help doctors to analyze and diagnose ophthalmological diseases, reduce the rate of misdiagnosis, improve the efficiency of diagnosis, and benefit human better. Our target user are hospitals as well as individual families, especially in remote areas where health care is not developed.
The realization of the whole system can be divided into four main aspects: the transplantation to the De10-Nano of the forward network, the training of network parameters, the collection of image samples and sample image enhancement and denoising.
![Image text](https://github.com/Johnhave/PR061/blob/master/realize_flow.png)
The Implementation Process of Artificial Intelligence Ophthalmology Diagnosis System
![Image text](https://github.com/Johnhave/PR061/blob/master/software_architecture.png)
Software Architecture
