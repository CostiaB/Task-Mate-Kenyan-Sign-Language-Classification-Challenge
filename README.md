# Task-Mate-Kenyan-Sign-Language-Classification-Challenge


Sign language competition at [Zindi](https://zindi.africa/competitions/kenyan-sign-language-classification-challenge/)

This is simple blending pipeline example, three models are used:
Regnet_x_8gf
ConvNext_base
EfficientNet-B3

Pipeline is following:


![Pipeline](/images/pipeline.jpg?raw=true)

Prior to training I have deleted some incorrect images. 
A small amount of transformations is used, but RandomCenterBlur is very helpful, because many images are fuzzy.

Transformation example:

![Pipeline](/images/example.png?raw=true)


In this example I used the same image size (320, 300)  and only one random split for each model. Number of epochs is not determined but training stops if validation loss does not improve during 7 epochs. 
