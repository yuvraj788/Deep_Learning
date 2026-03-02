# AI-Based Helmet Violation Detection 

---

##  **Problem Statement**

Road accidents caused by riders not wearing helmets are a major safety concern.  
Manual monitoring of helmet compliance is inefficient and error-prone.  
This project aims to build an **automated helmet detection** using **Deep Learning**.  
The model detects whether a motorcycle rider is wearing a **helmet** or **no helmet** from images using **Object Detection** techniques.

---

##  **Dataset**

This project uses the **YOLOv7 Helmet Detection Dataset** from **Kaggle**.

- The dataset contains labeled images of motorcycle riders.
- It includes **2 classes**: **helmet** and **no_helmet**.
- Images are organized into **train**, **validation**, and **test** folders.
- Annotations are provided in **YOLO format** (`class x_center y_center width height`).
- **Training Images:** 3546  
- **Validation Images:** 126  
---

##  **Model Used – YOLOv8**

In this project, we used **YOLOv8 (You Only Look Once – Version 8)** for object detection. YOLO is a **real-time object detection algorithm** that detects objects in a **single forward pass** through the network, making it extremely fast and efficient.  

## **YOLOv8**
YOLOv8 is a state-of-the-art, real-time computer vision model developed by Ultralytics (released in January 2023) designed for object detection, image segmentation, pose estimation, and classification. It is a single-stage, anchor-free detector known for high speed and accuracy, supporting various applications from drones to edge devices.


YOLO automatically optimizes:
- **Bounding Box Regression Loss**
- **Classification Loss**
- **Object Confidence Score**

The final trained model was saved as **`best.pt`** and used for prediction on test images.

---

## **Model Results**

After training for **50 epochs**, the model achieved the following performance:

###  **Overall Performance**

- **Precision:** 0.799  
- **Recall:** 0.804  
- **mAP@50:** 0.819  
- **mAP@50-95:** 0.387  

###  **Class-wise Performance**

| Class        | Precision | Recall | mAP@50 |
|-------------|----------|--------|--------|
| **Helmet**     | 0.834    | 0.900  | 0.904  |
| **No Helmet**  | 0.765    | 0.708  | 0.734  |

The model performs strongly in detecting **helmet-wearing riders** and shows good accuracy for **helmet violation detection**.

---
