---
title: "Work-Study Program (Alternance)"
date: 2024-09-25
draft: false

summary: "Deep Learning on Embedded Systems for Computer Vision"
tags: ["CNN", "Deep Learning", "Embedded Systems", "Computer Vision", "Professional Experience"]

thumbnail: "logo-keyia2.png"
thumbnailAlt: "Keyia Logo"

cover: "coverKeyia.png"
---

# Work-Study Program (Alternance)

## 🚀 Overview

After completing my internship at **Occion**, the company that had subcontracted me, **Keyia**, offered me a position in their work-study program (alternance) to continue advancing the **Strigoo** project. Strigoo is a sensor developed for detecting road actors such as pedestrians, bicycles, and vehicles. This opportunity allowed me to combine my final year of university studies with professional work, gaining hands-on experience in embedded systems and deep learning.

The goal was to implement a **deep learning algorithm** that would be more robust in detecting road actors. However, the hardware limitations posed a significant challenge: **1MB of RAM**! This constraint required innovative solutions to optimize the algorithm and make it feasible for deployment on embedded systems.

---

## 🛠️ Key Contributions

### 1. **Algorithm Optimization**
To address the hardware limitations, I implemented several optimization techniques:
- **Binarization**: Reduced the complexity of image processing.
- **Morphological Operations**: Improved image quality by removing noise and enhancing shapes.
- **Image Filters**: Applied various filters to make images lighter and faster to process.

### 2. **Deep Learning Architectures**
I explored and tested several neural network architectures to find the most efficient solution:
- **YOLOv8**: Known for its real-time object detection capabilities.
- **FOMO**: A lightweight model optimized for embedded systems.
- **MobileNetV2**: Designed for mobile and embedded devices with limited resources.
- **Custom Network**: A tailored architecture designed specifically for this project.

### 3. **Model Training and Deployment**
- Trained the models using a dataset of labeled images.
- Exported the models using **TensorFlow Lite** for deployment on embedded systems.
- Achieved an accuracy of **92%** with the custom network.
- Implemented **pruning** and **quantization** techniques to reduce the model size to under **1MB**, making it suitable for the microcontroller's limited resources.

---

## 📊 Results

- **Accuracy**: Achieved **92% accuracy** in detecting road actors.
- **Model Size**: Reduced the model size to under **1MB** using pruning and quantization.
- **Deployment**: Successfully implemented the model on the embedded system, enabling real-time detection.

---

## 🎓 Skills Acquired

This experience allowed me to develop a wide range of skills, including:
- **Deep Learning**: Understanding of neural network architectures, training, and optimization.
- **Computer Vision**: Techniques for image processing and object detection.
- **Embedded Systems**: Working with hardware constraints and optimizing algorithms for resource-limited environments.
- **MLOps**: Best practices for deploying and maintaining machine learning models.
- **Agile Methodology**: Collaborative development and iterative improvement.

---

## 🖼️ Custom Network Architecture

The final solution was based on a custom network architecture, similar to the one shown in the following diagram:

![Custom Network Architecture](red.jpg)

---

## 🌟 Conclusion

This work-study program was a transformative experience that allowed me to apply theoretical knowledge to real-world challenges. I gained expertise in deep learning, computer vision, and embedded systems, while also developing soft skills such as teamwork and project management. The successful implementation of the Strigoo sensor demonstrates the potential of combining academic learning with professional practice to create innovative solutions.

---

### 📌 Tags
#CNN #DeepLearning #EmbeddedSystems #ComputerVision #ProfessionalExperience