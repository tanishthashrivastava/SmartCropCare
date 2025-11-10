# SmartCropCare
# SmartCropCare: Image-based Plant Disease Classification with CNNs

**SmartCropCare** is a deep learning project that leverages Convolutional Neural Networks (CNNs) to automatically detect and classify plant leaf diseases from images. It was developed as part of an academic research project by students at the **School of Computer Applications, Lovely Professional University, Phagwara, Punjab, India**.

## Overview
The goal of this project is to assist in early and accurate identification of plant diseases to help farmers and agricultural experts make timely decisions. Using the *New Plant Diseases Dataset (Kaggle)*, which contains over **87,000 RGB images** of healthy and diseased plant leaves across **38 classes**, SmartCropCare builds and evaluates a CNN model capable of distinguishing among multiple crop diseases with high accuracy.

## Key Features
- Image preprocessing and augmentation to improve model robustness  
- Custom CNN architecture trained on augmented datasets  
- Multi-class classification across 38 plant species and diseases  
- Evaluation using accuracy, loss, confusion matrix, and F1-score  
- Visual analysis of correctly and incorrectly classified samples  
- Designed for future integration with mobile or edge-based systems  

## Technologies Used
- **Python**  
- **TensorFlow / Keras** for CNN model building  
- **Matplotlib & Seaborn** for data visualization  
- **Scikit-learn** for metrics and confusion matrix  
- **Google Colab** environment for GPU training  

##  Dataset
The project uses the **New Plant Diseases Dataset** available on [Kaggle](https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset).  
The dataset consists of:
- ~87,000 images (RGB, 256×256–512×512)
- 38 labeled classes (healthy + diseased leaves)
- Separate folders for training, validation, and testing

> Dataset not included in this repository due to large size.  
> Download it directly from Kaggle and extract it to `/tmp/cnn_project/` before running the notebook.

##  Model Architecture
The CNN model consists of:
- 3 × Conv2D layers with ReLU activation  
- MaxPooling2D for feature reduction  
- BatchNormalization and Dropout for stability and regularization  
- Dense (fully connected) layers ending with a Softmax layer (for 38 classes)

Optimizer: **Adam (lr = 1e-4)**  
Loss: **Categorical Crossentropy**  
Metrics: **Accuracy**  
Batch Size: **64**  
Epochs: **20**

## Results
| Metric | Value |
|--------|--------|
| Training Accuracy | ~83.8% |
| Validation Accuracy | ~77% |
| Test Accuracy | **76.87%** |
| Test Loss | **1.00** |

The model demonstrates good generalization with minimal overfitting, confirming the CNN’s ability to learn discriminative features for leaf disease detection.

##  Future Scope
- Integration of lightweight models like MobileNet or EfficientNet for mobile deployment  
- Expansion to real-world datasets with varied lighting and backgrounds  
- Incorporation of Explainable AI (Grad-CAM) for visual reasoning  
- Fusion with IoT sensor data for predictive disease management  


> 🌿 *"SmartCropCare — empowering sustainable agriculture through AI and deep learning."*

