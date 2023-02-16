# Yolov8 Sealnet

Yolov8 Sealnet is a seal face detection model built using Yolov8 that supports a downstream facial recognition model to enable non-invasive monitoring of seal populations. This Yolov8 model uses data stored in RoboFlow and leverages Weights & Biases for tracking model evaluation and performance metrics.

This repo contains two example notebooks that train a Yolov8 model on two different datasets:
* `sealnet-yolov8-colgate.example.ipynb` - This notebook is an example notebook that trains a Yolov8 model on data collected by Colgate University researchers. This data includes labelled images of harbour seal faces. This dataset has been carefully labelled in Roboflow and has a version where this data has been augmented to provide more training examples (and experiment with model resilience and performance).
* `sealnet-yolov8-unified.example.ipynb` - This example notebook also trains a Yolov8 model on a larger dataset that combines the data collected by Colgate University with external datasets of labelled fur seal faces from Roboflow Universe.

## Usage
To run these notebooks:
* Copy and/or rename the Jupyter notebooks and Roboflow API key files to remove `.example` from the file names.
* Copy your Roboflow API key into `roboflow.apikey`.
* Rename any of the Roboflow environment variables to make sure you are importing the right version of your dataset from the correct Roboflow workspace and project.
 
## Trained Models
To access the trained models, check out the `best.pt` files in the releases section of this repo. The release also includes the model performance and evaluation metrics and images for both the validation and test datasets. 