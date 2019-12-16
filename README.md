# Brainhack-til-ai-camp

## Description
A simple CNN model trained to classify 15 different human poses. Uses Xception with fine-tuning as base convolution and GAP + dense softmax as classifier block.
<br> Attained 81.25% accuracy for the final evaluation of TIL AI Camp 2019.
<br> Placed 4th out of 46 teams in the Polytechnic/University category.

## Instructions
Run train.ipynb to generate CNN model.
<br> Run evaluate.ipynb to test trained CNN model.

## Requirements
Keras 2.2.4+ & Tensorflow 1.13+
<br> Numpy

## Note
The notebooks work perfectly fine in the AWS platform using the conda-tensorflow-p36 kernel. They are not tested using other kernels, though they should work fine if the above requirements are met and the necessary dependencies are installed (with pip install).
