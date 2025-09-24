# distracted-driver-detection

This notebook demonstrates how to build a deep learning model to detect distracted driving behaviors from images. Below is a step-by-step summary of the workflow:

## 1. Data Loading and Exploration
- Load the dataset containing driver images and their labels.
- Explore the data to understand class distribution and check for missing values.
- Visualize the number of images per class and per subject.

## 2. Data Preparation
- Shuffle the dataset for randomness.
- Map class names (like 'c0', 'c1', etc.) to numeric labels.
- Convert images into arrays and save them for efficient loading.
- Rescale image data for better model performance.

## 3. Model Building
- Define the ResNet50 architecture using Keras.
- Implement identity and convolutional blocks for the ResNet structure.

## 4. Model Training and Evaluation
- Normalize the image data and prepare the labels.
- Use Leave-One-Group-Out cross-validation to evaluate model performance per driver.
- Train the model for different numbers of epochs and analyze training/testing accuracy and loss.

## 5. Final Model Training
- Train the final model on the full training set.
- Save and reload the trained model.

## 6. Prediction on Holdout/Test Data
- Load and preprocess the test images.
- Use the trained model to predict probabilities for each class.
- Save the predictions to a CSV file.

## 7. Visualization
- Visualize sample predictions to check model outputs.

---

This workflow helps in building a robust model for distracted driver detection using deep learning and provides insights at each step for better understanding and reproducibility.
