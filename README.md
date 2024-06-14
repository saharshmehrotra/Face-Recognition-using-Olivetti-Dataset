# Face Recognition with Olivetti Dataset

This project focuses on face recognition using the Olivetti dataset. The steps and methods utilized for face recognition in this study are outlined below.

## Table of Contents
1. [Face Recognition Process](#face-recognition-process)
2. [Face Recognition Overview](#face-recognition-overview)
3. [Olivetti Dataset Information](#olivetti-dataset-information)

## Face Recognition Process

The face recognition process for this project involves the following steps:

1. **Principal Component Analysis (PCA)**
   - Extract principal components from face images using PCA.
   
2. **Determine Adequate Number of Principal Components**
   - Identify the optimal number of principal components for the analysis.
   
3. **Model Evaluation**
   - Obtain accuracy scores using three different classification models.
   
4. **Cross-Validation**
   - Compute cross-validation accuracy scores for the three classification models.
   
5. **Parameter Optimization**
   - Perform parameter optimization for the best-performing model.

## Face Recognition Overview

The journey of automatic facial recognition systems began with the semi-automatic system developed by Bledsoe between 1964 and 1966. This early system involved manually identifying feature points on the face and then using a computer to classify these points. A significant advancement came in 1977 when Kanade developed the first fully functional facial recognition application using a feature-based approach. Over time, research in facial recognition has expanded, leading to significant advancements, particularly in two-dimensional (2D) and three-dimensional (3D) face recognition.

### 2D Face Recognition Approaches

2D face recognition approaches can be classified into three categories: analytical (feature-based, local), global (appearance-based), and hybrid methods.

- **Analytical Approaches**: These approaches recognize faces by comparing properties of facial components, such as distances and angles between feature points, shapes of facial features, or regional feature variables. They reduce computation costs by representing the face image with smaller data sizes.
  
- **Global Approaches**: These methods perform facial recognition without feature extraction, improving efficiency by using data derived from the entire face. Notably, Kirby and Sirovich (1990) developed the Eigenface method using Principal Component Analysis (PCA), which was further advanced by Turk and Pentland.
  
- **Hybrid Approaches**: Combining local and global approaches, hybrid methods aim to represent the face more accurately.

In this project, face recognition is assessed under global face recognition approaches, leveraging PCA to transform entire face images into vectors and compute eigenfaces from sample data. While PCA provides optimal data representation, it has limitations when dealing with different facial expressions and lighting conditions of the same person.

## Olivetti Dataset Information

The Olivetti Dataset, used in this project, contains face images collected between April 1992 and April 1994. Below are key details about the dataset:

- **Total Images**: 400 face images
- **Distinct Individuals**: 40 people
- **Images per Individual**: 10 different images
- **Image Variations**: Taken at different times with varying lighting, facial expressions, and facial details
- **Background**: All images have a black background
- **Image Properties**: Grayscale images with a size of 64x64 pixels
- **Pixel Value Scaling**: Pixel values scaled to the [0, 1] interval
- **Encoding**: Names of individuals encoded as integers from 0 to 39

This project utilizes these images to develop and evaluate facial recognition models.

---

For more details on the implementation and code, please refer to the project files and documentation.
