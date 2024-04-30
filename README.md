# ROP Classification using Pre-trained CNNs

GITHUB REPO LINK : https://github.com/mohammadshaad/early-detection-of-rop

## Overview

This repository contains the code and documentation for a study on the early detection of Retinopathy of Prematurity (ROP) using pre-trained convolutional neural network (CNN) models. ROP is a significant cause of childhood blindness, and early detection is crucial for effective treatment. The study explores the classification of different ROP stages using popular pre-trained CNN models such as InceptionV3, ResNet50, VGG16, VGG19, DenseNet201, MobileNet, and AlexNet.

## Instructions to Run the Code

To run the code in the accompanying ipynb file, follow these steps:

1. Install Jupyter Notebook if you haven't already. You can find installation instructions [here](https://jupyter.org/install).
2. Open a terminal or command prompt.
3. Navigate to the directory where the ipynb file is located using the `cd` command.
4. Launch Jupyter Notebook by running the command `jupyter notebook`.
5. In your web browser, Jupyter Notebook will open, displaying the file browser.
6. Click on the ipynb file to open it.
7. Run the code cells in the notebook by clicking on the "Run" button or using the keyboard shortcut Shift + Enter.



## Dataset

The dataset, sourced from Kaggle [link to dataset](https://www.kaggle.com/datasets/solennollivier/ropstages-reviewed), consists of 91 retinal fundus images categorized into four classes: Stage 1, Stage 2, Stage 3, and No ROP (absence of ROP). Each stage represents varying degrees of abnormal blood vessel growth in premature infants.

## Methodology

### 1. Image Preprocessing

Image preprocessing is crucial for enhancing raw images before analysis. MATLAB R2023a is used for implementing four preprocessing methods:

- **Histogram Equalization:** Enhances image contrast.
- **Canny Filter:** A widely used edge detection algorithm.
- **Sobel Filter:** Specifically used for edge detection in medical images.
- **Enhanced Multispectral Color Composite Images (EMCCI):** Combines information from multiple spectral bands.

### 2. Image Augmentation

Image augmentation involves applying various transformations to the existing dataset to create new training samples. MATLAB is used to implement augmentation techniques, including rotation, scaling, flipping, brightness adjustment, contrast adjustment, and random noise addition.

### 3. CNN Classification

The convolutional neural network (CNN) architecture includes convolutional layers, pooling layers, and fully connected layers. Pre-trained CNN models, including InceptionV3, ResNet50, VGG16, VGG19, DenseNet201, MobileNet, and AlexNet, are employed. The study compares the performance of these models on the preprocessed and augmented dataset.

## Results and Discussion

Results indicate that MobileNet, especially when using histogram equalization and enhanced multispectral color composite preprocessing, achieves the highest test accuracy of 97.67%. The study emphasizes the effectiveness of pre-trained models, image preprocessing, and augmentation in improving ROP classification accuracy.

## Conclusion

The study concludes that pre-trained models such as MobileNet, DenseNet201, and InceptionV3 outperform others in ROP classification. Specific preprocessing methods, like histogram equalization and enhanced multispectral color composite, contribute to higher accuracy. Future work could involve exploring real-time datasets, additional preprocessing methods, and alternative pre-trained models for further improvement.

Feel free to explore the code and documentation to gain insights into the implementation and findings of the study. Contributions and suggestions are welcome for enhancing the effectiveness of ROP classification using deep learning techniques.

## Detailed Documentation

For more detailed information, refer to the [Google Document](https://docs.google.com/document/d/1yM_PgIeN-airemnNor12O57eKrexeIYUDdxhMdlsWAk/edit?usp=sharing).
