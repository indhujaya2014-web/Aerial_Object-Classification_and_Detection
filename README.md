# Aerial Object Classification & Detection 🚁🦅  
## Overview  
A Deep Learning system to differentiate between birds and drones in aerial imagery to enhance airspace safety and wildlife monitoring. 
Build a deep learning system that:  
- Classifies aerial images as Bird or Drone  
- (Optional) Detects and localizes birds/drones using YOLOv8  
- Deploys the solution using Streamlit

**Domain Applications:**  
- Aerial Surveillance  
- Wildlife Monitoring  
- Security & Defense  
- Airport Safety & Bird-Strike Prevention  

## Tech Stack  
- **Deep Learning:** TensorFlow, Keras, YOLOv8
- **Computer Vision:** OpenCV, PIL
- **Deployment:** Streamlit
- **Analysis:** Matplotlib, Seaborn

## Dataset Understanding  
📂 Folder Structure (Classification)  
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

📂 Folder Structure (Object Detection)  
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

## Key Features
- **Binary Classification:** Custom CNN & MobileNetV2 (95%+ accuracy).
- **Object Detection:** YOLOv8 implementation for real-time bounding boxes.
- **Augmentation:** Applied rotation, zoom, and flip to handle diverse sky conditions.

## Results
| Model | Accuracy | Inference Time |
| :--- | :--- | :--- |
| Custom CNN | 89% | 45ms |
| MobileNetV2 | 96% | 20ms |
| YOLOv8 | 0.91 mAP | 12ms |

