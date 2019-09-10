# HiRES-Net-Accelerator-modeling
Surrogate modeling of complex accelerator system using Neural Network

**Accelerators are extremely complex systems** which involve a large number of parameters, non-linear behavior and many interactive systems.

Different scientific/beam physics applications call for highly
automated, rapid switching between different operational
modes.

Conventional numerical simulation methods are
computational expensive and too slow to be directly used
during operation.

**Neural Networks(NN)** can be used to perform **fast predictions** of various electron pulse properties as well as the 6-dimensional phase space using nondestructive measurements as inputs. 

<img src="https://drive.google.com/uc?export=view&id=1gQXb8ncaIFgdxj-ykyTrcmELTpA3Dc3_">


In this example, **TensorFlow/Keras** is used to build a **surrogate NN Model of the HiRES beamline**. A dataset of 2916 simulations is used for training and testing the model. From the machine learning point of view, this is formalized as a ***supervised learning problem***. Beamline parameters, such as RF gun phase and amplitude, buncher phase and amplitude as well as Solenoid current are inputs of the NN and the longitudinal phase space image is the output. The output is a continuous function of the input features so that it's a ***regression problem*** and ***Mean Square Error (MSE) loss function*** was choosen.
