# Facemask Detection Model for COVID-19

## Project Overview
This project focuses on developing a **Facemask Detection Model** to identify individuals wearing facemasks using deep learning techniques. The model is built on top of the pre-trained **MobileNetV2** architecture, leveraging its feature extraction capabilities.

## Key Features
- **Model Architecture**: 
  - Utilized **Keras (TensorFlow)** and **OpenCV** to implement the model.
  - Added a custom classification head on top of the pre-trained **MobileNetV2** model for binary classification (mask/no mask).
  
- **Training Strategy**: 
  - Frozen base model layers trained on **ImageNet** to retain learned features.
  - Only the new layers (Dense, Dropout) were trained to improve classification performance.
  - Applied an **80:20 train-test split** to evaluate model effectiveness.

- **Performance Metrics**: 
  - Achieved **99% accuracy** in just **20 epochs**.
  - Demonstrated high performance on both images and videos.

## Tools & Technologies
- **Python**: Programming language used for model development.
- **Keras**: For building and training the deep learning model.
- **TensorFlow**: Backend for Keras, providing the necessary computation framework.
- **OpenCV**: For image processing and handling video input.

## Results
The model successfully detects facemasks with high accuracy, contributing to efforts in managing public health during the COVID-19 pandemic.

