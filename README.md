# Face Recognition CNN Model

## Overview

This repository contains a Convolutional Neural Network (CNN) model for face recognition. The model was trained using a dataset from Kaggle, and it implements several techniques to enhance performance, including face cropping, data augmentation, and addressing class imbalance. The architecture used is ResNet50v2, which was fine-tuned and trained for 20 epochs.

## Dataset

The dataset used for training and validation was sourced from Kaggle. It consists of various images containing faces, which were preprocessed to improve the model's performance.

Link: https://www.kaggle.com/datasets/vasukipatel/face-recognition-dataset/data
## Preprocessing

### Face Cropping

To focus the model on the relevant parts of the images, faces were cropped from the images using the Haar Cascade classifier. This helped in reducing noise and improving the accuracy of the model.

### Addressing Class Imbalance

Class imbalance in the dataset was addressed using techniques such as oversampling the minority classes and undersampling the majority classes. This ensured that the model does not become biased towards any particular class.

### Data Augmentation

Data augmentation techniques were applied to artificially increase the size of the dataset and improve the robustness of the model. Techniques used include rotation, flipping, zooming, and shifting.

## Model Architecture

### ResNet50v2

The model architecture used is ResNet50v2, a powerful CNN architecture known for its deep layers and residual connections, which help in training deep networks by mitigating the vanishing gradient problem. The model was fine-tuned to adapt to the specific requirements of the face recognition task.

## Training

The model was trained for 20 epochs with the following results:
- **Training Accuracy:** 95.35%
- **Validation Accuracy:** 80.33%

## Evaluation

### Confusion Matrix

The confusion matrix was plotted to visualize the performance of the model in distinguishing between different classes. It provides insights into the types of errors the model is making.

### Classification Report

A classification report was generated to provide detailed metrics, including precision, recall, and F1-score for each class.

## Results

The model achieved a training accuracy of 95.35% and a validation accuracy of 80.33%. While the high training accuracy indicates that the model learned the training data well, the validation accuracy suggests that there is room for improvement in generalization to unseen data.

## Conclusion

This face recognition model demonstrates the effectiveness of using advanced CNN architectures like ResNet50v2 combined with preprocessing techniques such as face cropping and data augmentation. Future improvements could involve more extensive hyperparameter tuning, additional data augmentation strategies, or using more sophisticated methods to handle class imbalance.

