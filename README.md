# A Real Time Tomato Crop Disease Detection using Fine Tune Deep Learning

## Overview
This repository focuses on developing an advanced system for detecting diseases in tomato crops using real-time imaging and deep learning techniques. The solution is tailored to the agricultural context of India, where tomatoes are a vital crop. The system aims to address the shortcomings of existing methods by enhancing accuracy, generalization, and real-time applicability.

## Techniques and Algorithms
### 1. Convolutional Neural Networks (CNNs):
- The core of the model is a fine-tuned CNN designed to classify various tomato plant diseases. CNNs are effective for image-based tasks due to their ability to automatically and adaptively learn spatial hierarchies of features.
- The model is fine-tuned on a dataset of tomato leaf images with various diseases. Fine-tuning allows the model to adapt pre-trained weights from a general image classification model to the specific task of tomato disease detection, improving performance on this specific domain.
Image Processing:

### 2. OpenCV Integration:
- Used for real-time image acquisition and preprocessing. The system captures high-quality images from cameras, converts them to a uniform size, and applies enhancements like brightness and contrast adjustments.
Grayscale Conversion: To analyze the intensity and distribution of disease symptoms, images are converted to grayscale. This step is particularly useful for detecting fungal, bacterial, and parasitic infections.

### 3. Data Augmentation:
- To address the issue of limited training data, the repository employs data augmentation techniques. This includes random modifications such as cropping, rotating, and adjusting brightness, which helps the model generalize better by learning from a more diverse set of images.
Transfer Learning:
- The project leverages transfer learning by utilizing pre-trained models like AlexNet and VGG19, which have demonstrated high accuracy in similar tasks. This approach speeds up training and improves accuracy, especially when combined with a fine-tuning process.

### 4. Real-Time Analysis:
- The system is designed for real-time application, making it practical for use in actual agricultural settings. This is achieved through efficient image acquisition and processing pipelines, ensuring that the model can make quick and accurate predictions.

## Dataset
The dataset used consists of 10,000 images categorized into ten different classes, including both healthy and diseased leaves. These images are sourced from a publicly available Kaggle repository and include diseases like Bacterial Spot, Early Blight, and Yellow Leaf Curl Virus, among others.

## Accuracy and Performance
The model achieves high accuracy in classifying tomato plant diseases. For example, using models like AlexNet and VGG19, accuracies of 97.49% and 97.23% have been reported, respectively. Further performance improvements are made through fine-tuning and data augmentation. The system's design ensures it can handle variations in environmental conditions, making it robust and reliable for real-world applications.
