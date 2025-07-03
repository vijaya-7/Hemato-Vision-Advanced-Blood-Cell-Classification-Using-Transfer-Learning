# Hematovision: Advanced Blood Cell Classification Using Transfer Learning

### Author: Jakkam Vijaya lakshmi

---

## 🧬 Overview

Hematovision is a deep learning-based web application that performs automated blood cell classification using transfer learning. It uses the BCCD (Blood Cell Count and Detection) dataset to classify blood cells into four categories:

- Neutrophil  
- Eosinophil  
- Monocyte  
- Lymphocyte  

This application allows users to upload microscopic blood smear images and returns the predicted blood cell type with high accuracy.

---

## 📁 Dataset: BCCD

The BCCD Dataset is a labeled dataset for blood cell classification, organized in Pascal VOC format. It is suitable for object detection and classification tasks.

- Download: [BCCD Dataset Releases (.rec format)](https://github.com/Shenggan/BCCD_Dataset/releases)
- License: MIT

---

## 🧠 Model & Approach

- Utilizes transfer learning with pre-trained CNN models such as ResNet50, MobileNet, or EfficientNet.
- Trained on a labeled dataset of 12,500 microscopic blood cell images.
- Techniques used:  
  - Data augmentation  
  - Fine-tuning of pretrained layers  
  - Batch normalization and dropout  
- Produces fast and reliable predictions for real-world blood smear images.

---

## 🌐 Web App Workflow

The application is built using Flask, a lightweight Python web framework.

### 🔁 Workflow

1. User uploads a blood cell image.
2. The backend processes the image and passes it to the trained model.
3. The model returns the predicted class.
4. The result is displayed on the web interface.

---

## 🚀 Features

- Easy-to-use web interface
- Accurate classification of blood cell types
- Fast, real-time prediction
- Works with .jpg, .jpeg, .png images

---

## 🛠️ Tech Stack

- Language: Python  
- Framework: Flask  
- Deep Learning: TensorFlow / Keras or PyTorch  
- Frontend: HTML5, Bootstrap (optional)  
- Deployment: Localhost or Cloud Platforms (Render, Heroku, etc.)

---

## 📂 Folder Structure

hematovision/
├── static/
│ └── uploaded_images/ # Stores uploaded images
├── templates/
│ └── index.html # Frontend HTML file
├── model/
│ └── blood_cell_model.h5 # Trained model file
├── app.py # Flask application
├── requirements.txt # Python dependencies
└── README.md # Project documentation

