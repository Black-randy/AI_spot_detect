# <div align="center">YOLO Parking Spot detection model</div>

## <div align="left">Models</div>

## Overview

**Asiri Dhananjaya** | [LinkedIn](https://www.linkedin.com/in/asiri-bandara/) | [Github](https://github.com/Black-randy) |


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







## <div align="center"> Training </div>
The model was trained using a dataset of 23 drone-captured images, using the 2-fold cross-validation method due to the limited dataset size. To augment the dataset, we applied rotations of 30º and 60º, effectively tripling the number of training images. This augmentation improved the model’s ability to generalize across varying perspectives of the cars.

## DATA SET
This project makes it able to predict the number of available parking lots in a parking lot. The model used is yolov8 and fine-tuned on the parking lot dataset. The dataset is collected from [Kaggle](https://www.kaggle.com/datasets/blanderbuss/parking-lot-dataset). The dataset contains over 695,899 images.

## IoU Threshold
## Model Usage
## Example Workflow
## Model Comparison
## Conclusion
## Additional Information

## Results

The model were trained on GPU and took more than 8h to train and the results are shown below:

![input](results/zero_day/in-out/input.jpg)

![output](results/zero_day/in-out/output.jpg)

---

## License

This project is licensed under the MIT License. Feel free to use and modify the code for your own projects.

---