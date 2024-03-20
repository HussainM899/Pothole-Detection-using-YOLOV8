# Pothole Detection Using YOLOv8

## Project Overview
This project utilizes the YOLOv8 object detection model to identify potholes in road images, aiming to enhance road safety and maintenance efficiency by leveraging advanced AI techniques.

## Key Features
- High detection accuracy, enabling real-time pothole detection in diverse environments.
- Utilization of a robust, custom dataset from Roboflow, tailored for pothole identification.

## Technologies Used
- **Programming Language:** Python
- **Frameworks/Libraries:** Ultralytics YOLOv8, OpenCV, PyTorch
- **Dataset:** Custom pothole images dataset imported from Roboflow

## Getting Started
### Prerequisites
- Python 3.8+
- PyTorch 1.8+
- GPU with CUDA support for model training

### Installation
Clone the repository and install dependencies:

## Dataset
The project leverages a custom dataset from Roboflow, consisting of images specifically curated for pothole detection. This dataset ensures the model is trained on high-quality, relevant data, leading to improved accuracy and performance. Used this API code to get the dataset from the Roboflow website

```
!pip install roboflow
from roboflow import Roboflow
rf = Roboflow(api_key="IY7ESBtovhbLtT6jYb04")
project = rf.workspace("moinfaisal").project("potholes-detection-yolov8")
dataset = project.version(3).download("yolov5")
```


## Model Training
Training the YOLOv8 model involved:
- Customizing the dataset for optimal training performance.
- Monitoring training and validation loss to ensure model convergence.
- Utilizing best model weights for validation, ensuring robustness and reliability.

## Usage
Detail steps for using the model for inference, including code snippets or command line instructions.

## Contributing
Contributions to improve the model or extend its applications are welcome. Please follow the standard pull request process.

## Acknowledgments
Thanks to Roboflow for the dataset.
