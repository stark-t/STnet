# Slum Transfer Network (STnet)

In our study, we utilize both ResNet-50 and Xception to introduce the Slum Transfer Network (STnet). STnet is a custom CNN designed particularly for processing high-resolution remote sensing imagery.

## About STnet
The STnet draws its foundation from a heavily customized version of the Xception network1. A simplified schematic of the STnet is presented in Figure 1.

### Entry-flow
Comprises of five convolution combinations utilizing residual skip connections.
In recognition of the need to capture broader areas in high-resolution remote sensing imagery, the first two 2D convolutions employ large 9x9 kernels.
### Middle-flow
Employs feature pyramid pooling to establish a unified framework for feature extraction at diverse scales.
###Classification-flow
Composed of two linear functions.
Throughout the entire architecture of STnet, there's a harmonized use of batch-normalization followed by dropout layers. Cumulatively, the STnet comprises 22 layers with 3.3 million trainable parameters.

Figure 1: Simplified schematic of the STnet.

[Place image here or provide a link to the image]