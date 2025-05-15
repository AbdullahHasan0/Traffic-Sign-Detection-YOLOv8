# Traffic Sign Detection with YOLOv8
This project detects traffic signs (Speed Limit, Traffic Light, Crosswalk, Stop) using YOLOv8 on the [Road Sign Detection dataset](https://www.kaggle.com/datasets/andrewmvd/road-sign-detection). The model achieves a test mAP@50 of 0.908 with IoU=0.3 and confidence=0.1, optimized via grid search.

## Features
- Trained YOLOv8 Nano for 31 epochs with early stopping.
- Evaluated on 89 test images, with visualizations of predictions.
- Optimized for class imbalance (e.g., Traffic Light: 25 instances).

## Files
- `notebook/traffic_sign_detection.ipynb`: Kaggle notebook with preprocessing, training, and evaluation.
- `weights/best.pt`: Trained model weights.
- `visualizations/`: Prediction and ground truth images.
- `config/data.yaml`: Dataset configuration.

## Usage
Run the notebook in Kaggle with the dataset. Load `best.pt` for inference.

## License
MIT License
