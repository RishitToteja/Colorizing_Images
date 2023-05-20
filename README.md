# Colorizing_Images

Built and trained an autoencoder neural network in Keras with TensorFlow as backend. Autoencoder stores the input image representation in the latent space with very few dimensions compared to the input image.

The Decoder block of autoencoder consists of an output layer that gives the reconstructed image and some hidden layers, generally a combination of Convolutional Transpose Layers and Upsampling layers. In the Decoder block, the autoencoder learns the reconstruction of the original image from the previously learned latent space.

In this project, tweaked the Autoencoder Neural Network in such a manner that while training, we input Grayscale Images and set the output as their corresponding color images. In this way, the autoencoder layers would learn how to convert the latent space representation of grayscale images into colored images. For the Encoder, chose a pre-trained VGG16 model trained on ImageNet Dataset to classify 1000 classes. For the decoder part of the autoencoder, to upsample the latent representation up to the size of the original image used UpSampling Layers.

The project performed significantly well on converting grayscale images to colored rgb images. Some of the results can be seen below: 

![image](https://github.com/RishitToteja/Colorizing_Images/blob/main/Test%20Images/test_car.png)
![image](https://github.com/RishitToteja/Colorizing_Images/blob/main/Test%20Images/test_cat.png)
![image](https://github.com/RishitToteja/Colorizing_Images/blob/main/Test%20Images/test_dog_1.png)
![image](https://github.com/RishitToteja/Colorizing_Images/blob/main/Test%20Images/test_dog_2.png)
![image](https://github.com/RishitToteja/Colorizing_Images/blob/main/Test%20Images/test_flower_1.png)
![image](https://github.com/RishitToteja/Colorizing_Images/blob/main/Test%20Images/test_flower_2.png)
![image](https://github.com/RishitToteja/Colorizing_Images/blob/main/Test%20Images/test_person_female.png)
![image](https://github.com/RishitToteja/Colorizing_Images/blob/main/Test%20Images/test_person_male.png)
