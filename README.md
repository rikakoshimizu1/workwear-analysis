# Workwear Image Classification

## Overview
This project explores the use of **machine learning and deep learning** to classify clothing items based on their suitability for workwear using the `Fashion MNIST` dataset. The goal is to develop a classification system that identifies **work-appropriate and non-work-appropriate clothing** and to further distinguish specific clothing types using convolutional neural networks.

## Objective
To develop an image classification system using **TensorFlow** and neural networks to classify **grayscale images** of clothing items from the `Fashion MNIST` dataset as work-appropriate or not work-appropriate. The project involves preprocessing image data, creating binary labels, analyzing class distributions, training neural networks, and developing CNN-based classifiers for more detailed clothing classification.

## Dataset
The **Fashion MNIST** dataset contains 70,000 grayscale images of size 28x28 pixels, divided into:
 - Training set: `60,000` images
 - Test set: `10,000` images

Each image represents one of **10 fashion item categories**:
 - **0**: T-shirt/top
 - **1**: Trouser
 - **2**: Pullover
 - **3**: Dress
 - **4**: Coat
 - **5**: Sandal
 - **6**: Shirt
 - **7**: Sneaker
 - **8**: Bag
 - **9**: Ankle Boot

## Features
 - **Data Preprocessing**: Normalizing pixel values, reshaping image data, creating binary labels, and splitting data into training and validation sets.
 - **Class Distribution Analysis**: Analyzing the distribution of clothing categories and workwear classifications using `pandas` and `matplotlib`.
 - **Neural Network Classification**: Building and training a feedforward neural network using `TensorFlow` to classify clothing as work-appropriate or not work-appropriate.
 - **CNN Classification**: Developing convolutional neural networks to distinguish between specific clothing types within broader categories.
 - **Model Evaluation**: Evaluating training and validation accuracy and loss to measure model performance.
 - **Prediction Integration**: Combining predictions from the primary classifier and CNN-based classifiers for more detailed workwear classification.

## Model Performance
The primary neural network achieved:
 - **Training Accuracy**: `97.97%`
 - **Validation Accuracy**: `96.2%`

The model was trained using the `Adam` optimizer with `categorical_crossentropy` loss and evaluated using training and validation accuracy and loss.

## Challenges
 - Determining how to define **work-appropriate and non-work-appropriate** categories from the original Fashion MNIST labels.
 - Managing the differences between broad Fashion MNIST categories and more specific clothing types.
 - Developing additional CNN-based classifiers to provide more detailed classification within broader clothing categories.
 - Integrating predictions from multiple models while maintaining consistent workwear classifications.

## Analysis and Insights
This project demonstrated the importance of **data preprocessing and classification design** when applying machine learning to a real-world problem. Converting the original Fashion MNIST categories into binary workwear classifications provided a way to apply image classification to a practical use case. Developing additional CNN-based classifiers also demonstrated how specialized models can provide more detailed information when broad categories are not sufficient for the classification task.

## Future Improvements
Potential extensions to the project include:
 - Expanding the dataset beyond Fashion MNIST with real-world clothing images.
 - Developing models to analyze text, logos, and graphics on clothing to identify potentially inappropriate or profane content.
 - Increasing the number of clothing categories and classification criteria.
 - Improving CNN performance through additional hyperparameter tuning.
 - Developing an outfit recommendation system based on clothing classifications.

## About
This project was developed as an **independent machine learning project** using Python and TensorFlow. The project serves as a foundation for a future **workwear outfit recommendation system** by first establishing clothing classification based on workwear suitability.
