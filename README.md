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

![System Architecture](![Picture1](https://github.com/user-attachments/assets/5498d62f-d08c-4c64-ae50-97c01b7d118d)
)

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
![Image Detection](![Screenshot 2025-07-08 195847](https://github.com/user-attachments/assets/2d332a08-df3c-4e02-a94d-bc804fc35bdc)
)

### Video Detection  
![Video Detection](![Screenshot 2025-07-08 195902](https://github.com/user-attachments/assets/dd2a04a0-ef3c-4156-9601-0cf82cf2ee0d)
)

### Webcam Detection  
![Webcam Detection](![Screenshot 2025-07-08 200334](https://github.com/user-attachments/assets/db51fe4a-f027-4188-9a58-1c548de96876)
)

---


