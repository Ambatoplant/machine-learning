# Plant Classification with InceptionV3

This repository contains the code and documentation for building a plant classification model using InceptionV3, a pretrained convolutional neural network. The model is fine-tuned to classify 15 different plant species/classes.

## Table of Contents

- [Overview](#overview)
- [Classes](#classes)
- [Dataset](#dataset)
- [Requirements](#requirements)
- [Installation](#installation)
- [Results](#results)
  
## Overview

This project fine-tunes the InceptionV3 model for the task of multi-class plant classification. The model is trained on a dataset containing images of 15 plant species and is optimized for accuracy.

## Classes

The model is designed to classify the following plant species:

1. Sunflower (Bunga Matahari)
2. Pomegranate (Delima)
3. Wheat (Gandum)
4. Corn (Jagung)
5. Guava (Jambu Batu)
6. Cocoa (Kakao)
7. Frangipani (Kamboja)
8. Moringa (Kelor)
9. Aloe Vera (Lidah Buaya)
10. Jasmine (Melati)
11. Pineapple (Nanas)
12. Okra (Okra)
13. Cassava (Singkong)
14. Sorghum (Sorgum)
15. Tomato (Tomat)

## Dataset

Prepare a dataset with labeled images for the above classes. Organize the dataset into folders based on the species. Each species should have its own folder containing all the images for that class. For example:

```
/dataset
  /class_0
    image1.jpg
    image2.jpg
    ...
  /class_1
    image1.jpg
    image2.jpg
    ...
  ...
```

Ensure that the dataset contains a sufficient number of high-quality images for each class. During training, the script will automatically split the dataset into training and validation sets.

## Requirements

- Python >= 3.8
- TensorFlow >= 2.8
- NumPy
- Matplotlib
- Pillow

## Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/plant-classification.git
cd plant-classification
```

## Results

The model achieved the following performance metrics on the training dataset:

- Accuracy: **85%**
- Precision, Recall, and F1-score for each class can be computed using the `classification_report` function in scikit-learn.
