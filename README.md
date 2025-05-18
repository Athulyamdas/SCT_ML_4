# 🤚 Hand Gesture Recognition using CNN

This project focuses on recognizing hand gestures using a Convolutional Neural Network (CNN) trained on the LeapGestRecog dataset. The model can accurately classify 10 different hand gestures based on grayscale image inputs. The primary goal is to explore deep learning for human-computer interaction (HCI) using gesture recognition.

---

## 📌 Project Objective

To build a deep learning model that:
- Accepts grayscale images of hand gestures.
- Classifies them into one of 10 predefined gesture categories.
- Achieves high accuracy and generalizes well across different users.

---

## 🗃️ Dataset Overview

The dataset used is **LeapGestRecog**, which includes:
- Images from 10 different individuals.
- 10 gesture categories: palm, L, fist, fist_moved, thumb, index, ok, palm_moved, C, and down.
- Each gesture folder contains over 200 image samples per person.
- Images are in grayscale `.png` format with uniform dimensions.

---

## 🧠 Model Summary

A Convolutional Neural Network (CNN) architecture was used due to its effectiveness in image classification tasks. The model consists of:
- Convolutional and pooling layers to extract spatial features.
- Dense layers to learn gesture patterns.
- Dropout to prevent overfitting.
- A softmax output layer for multi-class classification.

The model is compiled with categorical cross-entropy loss and the Adam optimizer.

---

## 🧪 Workflow

1. **Data Preprocessing**
   - Images are loaded, resized to 64x64 pixels, and normalized.
   - Labels are encoded and one-hot encoded.
   - Dataset is split into training and testing sets.

2. **Model Training**
   - A CNN model is trained on the preprocessed data.
   - Trained for 15 epochs with validation monitoring.

3. **Evaluation**
   - Performance is evaluated using accuracy, classification reports, and a confusion matrix.
   - The model demonstrates strong classification accuracy across all gesture classes.

4. **Prediction**
   - A utility function allows for predicting the gesture shown in any new image input.

---

## 📈 Results

- Achieved high test accuracy across the 10 gesture classes.
- Demonstrated effective generalization to unseen test data.
- Visualized predictions using confusion matrix and classification reports.

---
