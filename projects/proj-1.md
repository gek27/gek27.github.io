---
layout: post
title: 'Deepstream Mask Detection'
---
This project was a CWRU funded project, training a ResNet-18 Neural Network with over 6000 images of facial data, both masked and unmasked individuals, to recognize and label faces using Nvidia's Deepstream technology. The system was based off of [Nvidia's mask-detection](https://github.com/NVIDIA-AI-IOT/face-mask-detection), however I retrained and pruned the model and Deepstream setup, to allow it to be more approachable and implementable on smaller scales. Their init

The model produced was light enough to be run on a Jetson Nano that could run at a theoretical 25 FPS from a camera feed, as featured [here](https://drive.google.com/file/d/1XhRk15QQzZ31rqxSyrsL2cB5Hokyi0yz/view?usp=sharing) This would allow a 'mask detection' system to be implemented in stores and University, to verify COVID-19 guidelines were being followed.

However - there were some roadblocks with this project. Notably the Jetson nano is not all that powerful. This resulted on the model running into throughput/input limits as well as causing the Nano to throttle during deepstream usage. This probably could be circumvented by further pruning the model, though that does come at the cost of accuracy. Alternatively a stronger GPU, such as that in the Xavier NX, could have been used.

{% include image.html image="projects/proj-1/shot1.jpg" %}

{% include image.html image="projects/proj-1/shot2.jpg" %}
