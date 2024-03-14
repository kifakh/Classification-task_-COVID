# COVID-19 Chest X-ray Classification

This repository contains a Convolutional Neural Network (CNN) model for classifying chest X-ray images into three categories: COVID-19, Normal, and Pneumonia.

## Dataset
The dataset used for training and evaluation consists of chest X-ray images collected from various sources. It includes images of patients diagnosed with COVID-19, as well as images of patients with normal chest conditions and those diagnosed with pneumonia.

## CNN Architecture
The CNN architecture used for classification is as follows:

- Input shape: (224, 224, 3)
- Convolutional Layer 1: 64 filters, kernel size (3,3), ReLU activation
- MaxPooling Layer 1
- Convolutional Layer 2: 128 filters, kernel size (3,3), ReLU activation
- MaxPooling Layer 2
- Dropout Layer (20% dropout rate)
- Convolutional Layer 3: 256 filters, kernel size (3,3), ReLU activation
- MaxPooling Layer 3
- Dropout Layer (20% dropout rate)
- Convolutional Layer 4: 512 filters, kernel size (3,3), ReLU activation
- MaxPooling Layer 4
- Dropout Layer (20% dropout rate)
- Flatten Layer
- Fully Connected Layer 1: 512 units, ReLU activation
- Dropout Layer (15% dropout rate)
- Output Layer: 3 units with softmax activation (for multi-class classification)

## Results
After training the model, the performance metrics such as accuracy, precision, recall, and F1-score are computed and reported. Additionally, confusion matrices and classification reports are generated for further analysis.

## Sample Predictions
Here are some sample predictions made by the trained model:

![COVID-19 X-ray](sample_predictions/covid19_xray.png)
*Prediction: COVID-19*

![Normal X-ray](sample_predictions/normal_xray.png)
*Prediction: Normal*

![Pneumonia X-ray](sample_predictions/pneumonia_xray.png)
*Prediction: Pneumonia*

## Conclusion
This project demonstrates the effectiveness of CNNs in classifying chest X-ray images for COVID-19 diagnosis. Further improvements and optimizations can be explored to enhance the model's performance.

For any inquiries or suggestions, feel free to contact the project maintainers.


