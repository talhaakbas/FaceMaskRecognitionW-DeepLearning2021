# FaceMaskRecognitionW-DeepLearning2021
This project is a deep learning-based face mask detection system developed using PyTorch. The goal is to classify whether a person in an image is wearing a mask or not, which can be helpful in enforcing safety protocols in public spaces or institutions during pandemics such as COVID-19.
📁 Dataset
We use the MaskedFace-Net dataset, specifically:

2863 Masked Images

1743 Non-Masked Images

These images are split into training and validation sets for model evaluation and generalization.

🔧 Project Workflow
1. Data Preparation
Image loading, resizing (100x100), and labeling (0: Non-Masked, 1: Masked)

Data augmentation and transformation using ToTensor()

2. Custom Dataset Class
A custom PyTorch Dataset class is implemented for structured data loading.

3. Model Architecture
Two CNN-based models (MaskDetection and MaskDetection1) are developed using:

Convolutional layers

ReLU activation

MaxPooling

Fully connected layers

4. Training and Validation
Data is transferred to GPU if available

Training and validation loops are handled using custom fit() and evaluate() functions

Accuracy and loss are monitored per epoch

5. Visualization
Accuracy and loss curves

Sample predictions

Confusion matrix for classification performance

6. Single Image Prediction
You can test the model on a new single image with GPU inference support

📊 Results
Training conducted over 4 epochs

Final validation accuracy and loss are displayed

Confusion matrix used for further analysis

💡 Key Libraries
PyTorch, Torchvision, OpenCV, NumPy, Matplotlib, Pandas

🚀 Run the Project
Clone this repo

Download the dataset to the specified folder

Run the notebook or script step-by-step
