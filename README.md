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
![Picture1](https://github.com/user-attachments/assets/35a88e78-e09a-4999-a6df-6c30db4a2c23)





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
![Screenshot 2025-07-08 195847](https://github.com/user-attachments/assets/65fba256-6f62-4af5-b96c-e0cf9e8f9faa)


### Video Detection  
![Screenshot 2025-07-08 195902](https://github.com/user-attachments/assets/759bef41-b713-41f5-9769-336bbf6d2c8f)


### Webcam Detection  
![Screenshot 2025-07-08 200334](https://github.com/user-attachments/assets/2e100704-f42b-42aa-a6b8-85b985cd884e)


---


