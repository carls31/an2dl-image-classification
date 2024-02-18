# Artificial Neural Networks and Deep Learning 2023 - Image Classification Challenge

This repository contains materials for the first Homework of the course [Artificial Neural Networks and Deep Learning](https://www11.ceda.polimi.it/schedaincarico/schedaincarico/controller/scheda_pubblica/SchedaPublic.do?&evn_default=evento&c_classe=810394&polij_device_category=DESKTOP&__pj0=0&__pj1=e1d18ec43fc9628f83ce82e5a309d240) at [Politecnico di Milano](https://www.polimi.it/).
The assignment focuses on binary image classification, specifically classifying plants into two categories based on their health state: "healthy" and "unhealthy." The task involves leveraging deep learning techniques to predict the correct class label for each image in the provided dataset.

## Dataset Details:
* Image size: 96x96
* Color space: RGB
* File Format: npz
* Binary Classes:
    * 0: "healthy"
    * 1: "unhealthy"
* Data: A numpy array of shape 5200x96x96x3, containing the RGB images.
* Labels: A 1-dimensional numpy array of shape 5200 with values in {'healthy', ‘unhealthy'}.

## Models Details:
The classification task employs a Transfer Learning approach with the ConvNeXtLarge model. The initialization is made with pre-trained weights followed by fine-tuning in two phases. 
To face the moderately-sized dataset some data augmentation techniques are applied, including:
* RandomFlip
* Crop 
* ZeroPadding 
* Brightness 
* Contrast

For a detailed understanding of the model architecture and techniques employed, please refer to the provided [Report](https://github.com/carls31/an2dl-image-classification/blob/main/Report.pdf).

## Results:
With the proposed model we obtained 4.5/5 in the challenge score. 
The model have been tested on an hidden dataset and it reached a 78% of accuracy.
