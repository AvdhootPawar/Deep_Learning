# Smart Road Maintenance with Deep Learning

## Project Overview

This project presents a deep learning-based system for real-time pothole detection using the YOLOv8 segmentation model. The system accurately identifies and marks potholes in road images, videos, and live webcam feeds through a user-friendly web interface. Designed with practicality in mind, it allows adjustable detection thresholds and delivers instant visual feedback, making it suitable for municipal authorities and road maintenance teams. The solution combines advanced object detection with a lightweight interface built using Streamlit, offering a scalable and efficient approach to modernizing road infrastructure maintenance.

---

## Key Features

- **Real-Time Pothole Detection**  
  Leverages YOLOv8 for fast and accurate detection of potholes in multiple input formats: images, videos, and webcam streams.

- **User-Friendly Interface**  
  Built with Streamlit, the interface enables media uploads, confidence threshold adjustments, and real-time visualization of results.

- **Segmentation Masks**  
  Detected potholes are highlighted using pink masks for clear and intuitive visual feedback.

- **Performance Metrics**  
  Displays quantitative metrics such as Precision, Recall, and mean Average Precision (mAP) to assess model performance.

- **Video Tracking with ByteTrack**  
  Ensures consistent pothole tracking across frames in video streams, even under occlusions or motion blur.

- **Scalable Design**  
  Built for real-world deployment on edge devices such as drones, dashcams, or Raspberry Pi.

---

## System Architecture

- **Input Module**  
  Accepts image and video file uploads or live webcam input.

- **Preprocessing Module**  
  Resizes inputs to 640×640 and normalizes pixel values for compatibility with the YOLOv8 model.

- **YOLOv8 Segmentation Engine**  
  Detects potholes and generates both bounding boxes and pixel-level segmentation masks.

- **Tracking Module (ByteTrack)**  
  Maintains consistent tracking IDs for potholes across consecutive video frames.

- **Postprocessing Module**  
  Overlays segmentation masks, bounding boxes, and labels onto the original input for visualization.

- **Streamlit UI**  
  Displays original and annotated outputs side-by-side, along with adjustable detection threshold and real-time statistics.

![System Architecture](https://media/image3.png)

---

## Results

The system was evaluated on a validation dataset and achieved the following performance metrics:

- **Precision**: 0.957  
- **Recall**: 0.887  
- **mAP@0.5**: 0.940  
- **mAP@0.5:0.95**: 0.832

---

## Sample Outputs

### Image Detection  
![Image Detection](https://media/image4.jpeg)

### Video Detection  
![Video Detection](https://media/image5.jpeg)

### Webcam Detection  
![Webcam Detection](https://media/image6.jpeg)

---


