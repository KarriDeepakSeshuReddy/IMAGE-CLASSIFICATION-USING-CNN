
Image Classification using Convolutional Neural Networks (CNN) : A Deep Learning Approach for Multi-Class Classification
Overview
This project demonstrates a deep learning approach for multi-class image classification using Convolutional Neural Networks (CNNs). The model classifies images into predefined categories such as airplanes, cars, cats, dogs, flowers, fruits, motorbikes, and people.

The project includes the following steps:

Data preprocessing (resizing, normalization, and augmentation).
Building and training a CNN model.
Evaluating performance using metrics like accuracy, precision, recall, F1-score, and confusion matrix.
Visualizing training history and model predictions.
Dataset
Total Images: ~6,000 training images and ~1,000 testing images.
Categories: Airplane, Car, Cat, Dog, Flower, Fruit, Motorbike, Person.
Format: JPEG.
Resolution: Resized to 150x150 pixels.
Dataset Link: https://www.kaggle.com/datasets/kkhandekar/image-dataset
Sample images from the dataset
Screenshot 2024-11-25 193948
Data Augmentation
Rotation range: 20°
Width and height shift: 0.2
Shear range: 0.2
Zoom range: 0.2
Horizontal flipping
Model Architecture
The CNN model consists of:

Conv2D Layers: 3 layers with increasing filter sizes (32, 64, 128).
Pooling: MaxPooling layers after each Conv2D layer.
Dropout: A dropout layer with a 50% rate to prevent overfitting.
Fully Connected Layers:
Flatten layer.
Dense layer with 128 neurons and ReLU activation.
Output layer with softmax activation for multi-class classification.
Screenshot 2024-11-27 114819

Training Details
Optimizer: Adam
Loss Function: Categorical Crossentropy
Metrics: Accuracy
Epochs: 10
Batch Size: 32
Results
Training Accuracy: 84.10%
Validation Accuracy: 90.96%
Test Accuracy: ~89%
Evaluation Metrics:
Precision, Recall, and F1-scores reported for each class.
Confusion matrix visualization.
Screenshot 2024-11-25 205113
Graph comparing Model Accuracy and Model Loss

Visualizations
Training History:
Accuracy and Loss curves.
Sample Predictions:
Random images from each class with predictions and confidence.
Classification Report:
Heatmap of precision, recall, and F1-scores.
Screenshot 2024-11-25 205128 Screenshot 2024-11-27 113746
Screenshot 2024-11-25 205140

Confusion Matrix:

Matrix visualizing true vs predicted labels.
Screenshot 2024-11-25 205154
Prediction Confidence:

The model’s predictions for test images included confidence percentages for each class.
Screenshot 2024-11-25 205211

How to Run
Clone the repository and upload the dataset.
Install dependencies: pip install tensorflow sklearn matplotlib seaborn.
Execute the notebook ML_2(final_project).ipynb in Google Colab or a local Jupyter environment.
Save the trained model: image_classification_model.h5.
Future Work
Transfer Learning: Utilize pre-trained models like ResNet or Inception for better accuracy.
Advanced Augmentation: Apply Mixup or Cutout techniques.
Real-time Inference: Optimize the model for deployment in real-time applications.
