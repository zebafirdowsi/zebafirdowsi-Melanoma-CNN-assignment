# Melanoma-CNN-assignment
# `Skin Cancer Classification`


## Problem Statement
In this assignment, you will build a multiclass classification model using a custom convolutional neural network in tensorflow.

`Problem statement`: To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant. The data set contains the following diseases:

## Dataset
The dataset contains 2357 images of malignant and benign oncological diseases, sourced from the International Skin Imaging Collaboration (ISIC). The dataset is divided into the following classes:
- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

## Project Pipeline
1. **Data Reading/Data Understanding:** Define the path for train and test images.
2. **Dataset Creation:** Create train and validation datasets from the train directory with a batch size of 32. Resize images to 180x180.
3. **Dataset Visualization:** Visualize one instance of all nine classes present in the dataset.
4. **Model Building & Training:** 
    - Create a CNN model for multiclass classification.
    - Rescale images to normalize pixel values between 0 and 1.
    - Choose an appropriate optimizer and loss function.
    - Train the model for ~20 epochs.
    - Evaluate model performance and analyze for underfitting/overfitting.
5. **Data Augmentation:** Choose an appropriate data augmentation strategy to resolve underfitting/overfitting observed in the previous step.
6. **Model Building & Training on Augmented Data:** 
    - Train the CNN model on augmented data.
    - Evaluate model performance and analyze for improvements.
7. **Class Distribution Analysis:** Examine the current class distribution in the training dataset.
    - Identify the class with the least number of samples.
    - Determine classes dominating the data in terms of proportionate number of samples.
8. **Handling Class Imbalances:** Rectify class imbalances present in the training dataset using Augmentor library.
9. **Model Building & Training on Balanced Data:** 
    - Train the CNN model on the rectified class imbalance data.
    - Evaluate model performance and analyze for improvements.

## Files Included
- `main.ipynb`: Jupyter notebook containing the code implementation of the project.
- `README.md`: Markdown file providing an overview of the project and its pipeline.
