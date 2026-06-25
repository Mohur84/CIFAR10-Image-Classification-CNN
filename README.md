CIFAR-10 Image Classification using Convolutional Neural Networks (CNN)
Project Overview

This project presents a complete implementation of a Convolutional Neural Network (CNN) for image classification using the CIFAR-10 dataset. The model is developed entirely using TensorFlow and Keras, demonstrating the complete deep learning workflow—from preprocessing the dataset to training, evaluating, and saving the final model.

The CNN learns meaningful image features automatically through multiple convolutional layers and predicts one of the ten object categories with high accuracy.

Objectives
Build a CNN from scratch using TensorFlow/Keras.
Perform image preprocessing and normalization.
Improve generalization using Batch Normalization and Dropout.
Reduce overfitting using Data Augmentation.
Train and evaluate the model efficiently.
Visualize learning curves and classification performance.
Save the trained model for future inference.

Dataset
Dataset: CIFAR-10

Official Website:
https://www.cs.toronto.edu/~kriz/cifar.html

Dataset Information
Property	Value
Total Images	60,000
Training Images	50,000
Testing Images	10,000
Image Size	32 × 32 Pixels
Color Channels	RGB
Number of Classes	10
CIFAR-10 Classes
ID	Class
0	✈ Airplane
1	🚗 Automobile
2	🐦 Bird
3	🐱 Cat
4	🦌 Deer
5	🐶 Dog
6	🐸 Frog
7	🐴 Horse
8	🚢 Ship
9	🚚 Truck

CNN Architecture
Input (32×32×3)

│
├── Conv2D (32 Filters, 3×3, ReLU)
├── Batch Normalization
├── Conv2D (32 Filters)
├── MaxPooling2D
├── Dropout

│
├── Conv2D (64 Filters)
├── Batch Normalization
├── Conv2D (64 Filters)
├── MaxPooling2D
├── Dropout

│
├── Conv2D (128 Filters)
├── Batch Normalization
├── MaxPooling2D
├── Dropout

│
├── Flatten

│
├── Dense (256)
├── Dropout

│
└── Dense (10)
        ↓
     Softmax

Features
✅ TensorFlow 2.x & Keras Sequential API
✅ Custom CNN Architecture
✅ Batch Normalization
✅ Dropout Regularization
✅ Image Normalization
✅ Data Augmentation
✅ Early Stopping
✅ ReduceLROnPlateau Callback
✅ Model Checkpointing
✅ Accuracy & Loss Visualization
✅ Confusion Matrix
✅ Classification Report
✅ Prediction on New Images
✅ Saved Trained Model

Model Performance

Metric	Result
Framework	TensorFlow 2.21
Model	Custom CNN
Training Images	50,000
Testing Images	10,000
Optimizer	Adam
Loss Function	Sparse Categorical Crossentropy
Test Accuracy	≈80%

Note: Actual accuracy may vary slightly depending on hardware configuration, TensorFlow version, and random initialization.

Training Workflow

Load CIFAR-10 Dataset
          │
          ▼
Normalize Images
          │
          ▼
Data Augmentation
          │
          ▼
Build CNN Model
          │
          ▼
Compile Model
          │
          ▼
Train Network
          │
          ▼
Evaluate Performance
          │
          ▼
Generate Metrics
          │
          ▼
Save Final Model

Generated Outputs
After training, the project automatically generates:

📷 Sample Training Images
📈 Accuracy vs Epoch Graph
📉 Loss vs Epoch Graph
📊 Confusion Matrix
📄 Classification Report
🔍 Sample Predictions
💾 Saved CNN Model

Example output directory:

assets/
│
├── sample_images.png
├── training_history.png
├── confusion_matrix.png
├── prediction_1.png
├── prediction_5.png
└── prediction_9.png
CIFAR10-Image-Classification-CNN/

Installation
Clone the repository

git clone https://github.com/YOUR_USERNAME/CIFAR10-Image-Classification-CNN.git

Navigate to the project folder

cd CIFAR10-Image-Classification-CNN

Install the required dependencies

pip install -r requirements.txt
▶ Running the Project

Run the Python script

python src/cifar10_cnn.py

Or open the notebook
notebook/CIFAR10_CNN.ipynb

and execute all cells using:

Jupyter Notebook
JupyterLab
VS Code
Google Colab
Saving and Loading the Model

The trained model is automatically saved as:

model/cifar10_final_model.keras

Load the model later without retraining:

import tensorflow as tf

model = tf.keras.models.load_model(
    "model/cifar10_final_model.keras"
)

Technologies Used

Python
TensorFlow
Keras
NumPy
Matplotlib
Seaborn
Scikit-learn
Jupyter Notebook

Future Enhancements

Transfer Learning using ResNet50
EfficientNet Implementation
MobileNetV2 Integration
TensorBoard Visualization
Hyperparameter Optimization
Flask REST API
Streamlit Web Application
Docker Containerization
ONNX Model Export
Real-Time Webcam Prediction

Author
Mohur Datta
B.Tech – Computer Science & Engineering (Artificial Intelligence & Machine Learning)
VIT Bhopal University
Registration Number: 23BAI11091

Contributing
Contributions are welcome!

If you would like to improve this project:

Fork the repository
Create a feature branch
Commit your changes
Push the branch
Open a Pull Request

License
This project is distributed under the MIT License.
Feel free to use, modify, and distribute this project for educational and research purposes.

Support
If you found this project useful, please consider giving it a ⭐ Star on GitHub.

Your support motivates future development and helps others discover this project.
