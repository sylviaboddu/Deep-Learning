# Image Colorization using Deep Neural Networks


# Simple Convoloutional Neural Network

This is a very basic model to do the coloring, the architecture is very simple as shown in the below diagram. The black and white images are in gray scales. They range from 0-225. To choose the accurate color we convert the input layer of gray scale to two layers of colored layers we use convolution layers.  

Each filter can add or remove some information, the network can combine these filters or select filters to form a new image. CNNs adjust the filters to obtain better results. lot of filters are stacked to form 2 layers ‘a’ and ‘b’. Predicted values and the real values that fall under the same interval are mapped which are ranging from -1 to 1. TanH function is used for mapping. From the Gray scale input layers the outputs are mapped to these Lab color layers and they are normalized, after that the errors are calculated the network updated, the same process is repeated till the error value reduces to the max. 

<img src="https://media.github.iu.edu/user/22196/files/79f67496-29e5-4f11-90a7-552184b59d22" width="700">


# CNN with Encoder Decoder 

While the model primarily constitutes an encoder and a decoder, it also comprises of an immensely powerful image classification network ‘InceptionResNetv2’ used for transfer learning. The Inception model has been trained on over a million images from the ImageNet database and helps in classifying a particular image into one of 1000 categories. The combined model, as such comprises of the Inception network, the encoder model, their merged model, and a decoder model. 


## AutoEncoder Architecture
<img src="https://media.github.iu.edu/user/22196/files/4527352d-cd32-41f6-9537-610fdeb686b0" width="700">


# GAN

Generative Adversarial Neural Network is a type of Image generation model. In GANs, one model, generator tries to generate the image while another model, discriminator tries to find out if the image is generated by the generator or not. The goal of the generator here is to fool the discriminator. To achieve that goal, the generator has to generate images that are closer to the ground truth. Every time, the discriminator correctly identifies that the generator has created the image, the generator updates its weights to try to generate a better image to fool the discriminator.

## Generator Architecture
<img src="https://media.github.iu.edu/user/22196/files/c7277b28-737c-4178-9534-29b1892565d1" width="700">

## Discriminator Architecture
<img src="https://media.github.iu.edu/user/22196/files/b90eabc8-4cc8-42bd-8580-74a24fb2ded7" width="700">

# Results


## 2-D CNNs
<img src="https://media.github.iu.edu/user/22196/files/0ea88c10-7454-46fe-8166-6a54ae084b97" width="700">

## GANs
<img src="https://media.github.iu.edu/user/22196/files/19a8d01b-7a7b-48d2-8438-9c288ee395df" width="700">
<img src="https://media.github.iu.edu/user/22196/files/d6554240-addb-43e9-91dc-1c881652439e" width="700">
<img src="https://media.github.iu.edu/user/22196/files/230ab2b5-0453-4e41-9868-020f70da5c51" width="700">

