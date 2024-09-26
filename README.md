# <div align="center">YOLO Parking Spot detection model</div>

## <div align="left">Models</div>

## Overview
This repository hosts a YOLO-based Parking Spot Detection Model aimed at real-time detection of available parking spots using drone and CCTV footage. The model has been trained and fine-tuned using YOLOv8, a state-of-the-art object detection algorithm, and optimized for real-time applications in urban environments.

Author: **Asiri Dhananjaya** | [LinkedIn](https://www.linkedin.com/in/asiri-bandara/) | [Github](https://github.com/Black-randy) |


##  YOLO 
YOLO (You Only Look Once) is an advanced object detection algorithm designed for real-time applications due to its exceptional speed and accuracy. In this project, we trained models using YOLOv8n.
br>

<img width="1024" src="https://raw.githubusercontent.com/ultralytics/assets/main/im/banner-tasks.png" alt="Ultralytics YOLO supported tasks">


<br>

<details open><summary>Detection </summary>

<div align="center">

| Model                                                                                | size<br><sup>(pixels) | mAP<sup>val<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
| ------------------------------------------------------------------------------------ | --------------------- | -------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8n.pt) | 640                   | 37.3                 | 80.4                           | 0.99                                | 3.2                | 8.7               |


</div>

<br>







## <div align="center"> Model Training </div>


The yolov8n_plp_100e models were trained using the [PKLot Dataset](https://www.kaggle.com/datasets/blanderbuss/parking-lot-dataset), which contains over 695,000 labeled images of parking spaces captured under various weather conditions (sunny, overcast, rainy). 

---

#### PKLot Dataset
The PKLot Dataset consists of 695,899 images of parking spaces, labeled as vacant or occupied. The dataset includes images taken under sunny, overcast, and rainy conditions, allowing the model to generalize well to different lighting and weather scenarios. This real-world dataset is ideal for testing parking space detection models.

---

## System Architecture

The system architecture involves real-time video feed processing from strategically placed cameras (CCTV) or drone footage to detect parking spaces. The YOLO model identifies available spots, processes the images, and sends real-time notifications via a mobile application.

Key features:
- **Real-time object detection**: Continuous monitoring of parking lots with high-definition cameras or drones.
- **Mobile integration**: User-friendly interface with real-time notifications of available parking spaces.

---

## Results

The model was trained on a GPU with a training time of over 8 hours, yielding impressive real-time detection results. Below are sample outputs of the model, showing before and after applying the YOLO model to detect vacant parking spots:

| Input Image                           | Output Image                         |
|---------------------------------------|--------------------------------------|
| ![Input](results/zero_day/in-out/input.jpg) | ![Output](results/zero_day/in-out/output.jpg) |

---

## License

This project is licensed under the **MIT License**. Feel free to use, modify, and distribute the code and models for personal and commercial projects, as long as the original author is credited.

---

For more details, visit the original repository: [AI Spot Detection](https://github.com/Black-randy/AI_spot_detect).

---