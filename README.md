# Masked Autoencoders for Adversarial Purification

This repo contains the code for our CSCI 566 - Deep Learning course project. We propose the defense method of using a generative model to purify adversarial images prior to classification, also known as adversarial purification. Through the use of finetuned Masked Autoencoders, we can learn a latent space that will undo the mutations to the image and output a purified reconstruction. These reconstructed images will then be classified to the target label of the unaltered image, thus rendering the adversarial attack futile. Our experiments showed that MAEs have some potential for adversarial purification.

Our experiments were performed on the ImageNet dataset. We used Gaussian noise and FGSM attack to generate noisy images. For classification, we used ViT Base Patch 16 image classifier. This repository contains the code for creation of the dataset, fine-tuning of the MAE, generation of the reconstructed images and image classification. Our experiments were performed on Google Colab Pro and Google Cloud.

For downloading the fine-tuned models: click [here](https://drive.google.com/drive/folders/1Dj_nhXOVIibm9ThWV2vuR7ttb0LvqQZp?usp=share_link)

Contributors:
 - Prashanth Ravichandar
 - Alex Korman
 - Siddharth Byale
 - Julianne Guo