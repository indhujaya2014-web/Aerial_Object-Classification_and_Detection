# Aerial Object Classification & Detection 🚁🦅  
📌 **Overview**  
A Deep Learning system to differentiate between birds and drones in aerial imagery to enhance airspace safety and wildlife monitoring. 
Build a deep learning system that:  
- Classifies aerial images as Bird or Drone  
- (Optional) Detects and localizes birds/drones using YOLOv8  
- Deploys the solution using Streamlit

🌿**Domain Applications:**  
- Aerial Surveillance  
- Wildlife Monitoring  
- Security & Defense  
- Airport Safety & Bird-Strike Prevention  

🛠️ **Tech Stack**  
- **Deep Learning:** TensorFlow, Keras, YOLOv8
- **Computer Vision:** OpenCV, PIL
- **Deployment:** Streamlit
- **Analysis:** Matplotlib, Seaborn

## Dataset Understanding  
📂 Folder Structure [Classification](https://drive.google.com/drive/folders/1nn1vqsh8juhafkJcleembrjQ9EqtIoMh?usp=sharing)  
classification_dataset/  
│  
├── train/  
│   ├── bird/  
│   └── drone/  
├── valid/  
│   ├── bird/  
│   └── drone/  
└── test/  
    ├── bird/  
    └── drone/   

📂 Folder Structure [Object Detection](https://drive.google.com/drive/folders/114wV_igIhWldcG0HftNIZZsivrs8G22p?usp=sharing)  
object_detection_Dataset/  
│  
├── images/  
│   ├── train/   (2662 images)  
│   ├── val/     (442 images)  
│   └── test/    (215 images)  
│  
├── labels/  
│   ├── train/   (2662 .txt files)  
│   ├── val/     (442 .txt files)  
│   └── test/    (215 .txt files)  


🔍 **Key Features**  
- **Binary Classification:** Custom CNN & MobileNet (95%+ accuracy).
- **Object Detection:** YOLOv8 implementation for real-time bounding boxes.
- **Augmentation:** Applied rotation, zoom, and flip to handle diverse sky conditions.

## Streamlit Application Features

The Streamlit app provides an interface where you can:

*   **Select Task**: Choose between "Classification (Keras)" or "Object Detection (YOLOv8)".
*   **Upload Image**: Upload an aerial image for analysis.
*   **Classification (Keras)**: The best performing classification model (`best_model.h5`) will predict whether the image contains a "Bird" or a "Drone" and display the confidence score.
*   **Object Detection (YOLOv8)**: The YOLOv8 model will detect and localize all instances of "Bird" and "Drone" in the uploaded image, displaying bounding boxes and confidence scores.

🚀 **Results**  
| Model | Accuracy / mAP | Training Time (s) |
| :--- | :--- | :--- |
| Custom CNN | 0.8512 Accuracy | 754.94 |
| Transfer Learning (MobileNet) | 0.9814 Accuracy | 732.22 |
| YOLOv8 Object Detection | 0.820 mAP50 | 50 Epochs |
