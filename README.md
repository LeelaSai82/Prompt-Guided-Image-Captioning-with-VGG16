# Prompt-Guided-Image-Captioning-with-VGG16

📌 Project Overview
This project presents a system where users can submit images, and the system generates descriptive captions based on the image content using natural language queries. The model leverages VGG16 for feature extraction and YOLOv8 for activity recognition. This approach enhances interaction between visual data and contextual inquiries, making it useful for applications in accessibility technology, media analysis, and surveillance.

![image](https://github.com/user-attachments/assets/e0dc5d2d-a7ec-480d-b591-262231da7e21)


🚀 Features
✅ Image Upload & Processing: Users can upload images for automatic caption generation.
✅ Deep Learning-Based Captioning: Uses VGG16 for feature extraction and YOLOv8 for activity recognition.
✅ Natural Language Query Support: Users can ask context-based questions about the image.
✅ Real-Time Analysis: Capable of detecting specific activities like "sleeping" and "suspicious behavior."
✅ User-Friendly Frontend: Built using Flask, ensuring an intuitive experience.

🛠️ Tech Stack
Backend: Flask, Python
Deep Learning Models: VGG16, YOLOv8
Dataset Annotation & Processing: Roboflow
Libraries: TensorFlow/Keras, OpenCV, NumPy, Pandas

📂 Dataset
The dataset was collected through video recordings at the Eye-Tracking Lab, Amrita School of Engineering, using three cameras. Frames were extracted at 1 FPS and annotated with two key classes:
Class 1: Sleeping behavior
Class 0: Suspicious activity
Annotations were formatted for YOLOv8 for real-time object detection.

📊 Methodology
Image Upload: Users upload an image through the Flask-based interface.
Preprocessing: The image undergoes resizing, grayscale conversion, and feature extraction.
Feature Extraction:
VGG16 extracts visual features and identifies objects.
YOLOv8 detects activities like "sleeping" or "suspicious behavior."
Natural Language Processing: Analyzes user queries for logical and contextual optimization.
Caption Generation: Combines extracted features with user queries to generate context-based descriptions.
Output Generation: The final response is displayed to the user with labeled bounding boxes.

📈 Results
Model Accuracy: Achieved 96% accuracy in detecting suspicious activities.
Performance: High precision in activity classification, with minor misclassifications in background activities.
Potential Enhancements: Data augmentation, feature engineering, and model architecture improvements.
