# 📝 Concrete Crack Classification – README

## 📌 Project Overview
Cracks in concrete structures can compromise the safety and durability of buildings if left undetected. This project aims to develop a deep learning-based image classification model that can automatically detect concrete cracks, potentially preventing structural failures and saving lives. Using transfer learning and convolutional neural networks (CNNs), the model is trained to classify concrete images as cracked or non-cracked. The goal is to achieve 90%+ accuracy while ensuring the model does not overfit.

## 📂 Dataset
Dataset Source: Concrete Crack Dataset – Mendeley Data
Link: https://data.mendeley.com/datasets/5y9wdsg2zt/2 
The dataset consists of concrete images with visible cracks, collected from various buildings on the METU Campus. It is organized into two categories: negative (no cracks) and positive (with cracks) for image classification.For this project, the dataset was downloaded from the source and extracted. The folder was renamed to "concrete_dataset", with the "negative" category renamed to "without_cracks" and the "positive" category renamed to "with_cracks" for better clarity.

## ⚙️ Machine Learning Workflow
This project follows a structured ML workflow:

### Problem Formulation

1. Define the problem: Classify concrete as cracked or non-cracked.
2. Set success criteria: Achieve >90% accuracy while avoiding overfitting.

### Data Preparation

1. Load the dataset using Keras image_dataset_from_directory.
2. Perform data augmentation.
3. Split data into training (70%), validation (15%), and test (15%) sets.

### Model Development

1. Implement CNN-based transfer learning (MobileNetV2).
2. Fine-tune the model to optimize performance.

### Model Evaluation

1. Monitor training and validation accuracy/loss curves.
2. Ensure no overfitting using early stopping.

### Model Deployment & Prediction

1. Save the trained model.
2. Deploy the model to classify test images.

## ⚙️ Model Architecture

![Model](img\model.png)

## 📊 Training Process & Model Performance

![First model](img\accuracy_1.png)

![First model](img\loss_1.png)

![Second model](img\accuracy_2.png)

![Second model](img\loss_2.png)

![Second model](img\learning_rate.png)
