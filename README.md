# Solar Panel Object Detection Project

## Overview and Drive Link of Code
https://drive.google.com/drive/u/0/folders/1chptPgD7wqu6GWQV-6J4gQLz0yWROcXv

This project focuses on object detection of solar panels using deep learning models, specifically leveraging the YOLOv8 model. It involves dataset preparation, model training, evaluation, and inference.


## Directory Structure

```
📂 Project Root
├── images/                    # Contains image data used for training, validation, and testing
│   ├── image_chips_native-*   # Subfolder storing preprocessed image chips
├── labels/                    # Holds annotation files in YOLO format
├── mlruns/                    # Stores logs and metadata for MLflow tracking
├── train/                     # Training images and labels
├── val/                       # Validation images and labels
├── test/                      # Test images and labels for evaluation
├── solar_dataset.yaml         # Dataset configuration file for YOLO training
├── solar-p-detection.ipynb    # Jupyter Notebook for model training and evaluation
├── solar-panel.ipynb          # Jupyter Notebook for visualization and performance analysis
└── yolov8n.pt                 # Pretrained YOLOv8 model weights
```

## Workflow

### 1. Dataset Preparation

- Organize images and annotation files.
- Convert dataset into YOLO format if necessary.
- Update `solar_dataset.yaml` with dataset paths and class details.

### 2. Model Training

- Load YOLOv8 model (`yolov8n.pt`).
- Train using `solar-p-detection.ipynb`.
- Log training performance using MLflow.

### 3. Evaluation

- Compute metrics (IoU, mAP) using Pascal VOC and COCO methods.
- Analyze results in `solar-panel.ipynb`.

### 4. Inference & Deployment

- Run detection on test images.
- Deploy the model for real-time solar panel detection.

## Dependencies

- Python 3.x
- Ultralytics YOLOv8
- OpenCV
- Pandas
- Matplotlib
- MLflow
- Shapely (for IoU calculation)
- supervision (for evaluation metrics)

## Future Scope

- Improve model accuracy with data augmentation.
- Optimize inference for real-time applications.
- Integrate the detection pipeline with IoT-based solar panel monitoring systems.

---

**Author:** Ashutosh Ranjan\
**Date:** February 2025

