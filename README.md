# forest-type-mapping-ESP32
"A neural network model for forest type classification using multi-temporal remote sensing data, trained on spectral data and optimized for deployment on ESP32 with TensorFlow Lite."

This repository contains a project for forest type mapping using a neural network model, trained on multi-temporal spectral data of a forested area in Japan. The model is optimized for deployment on an ESP32 microcontroller using TensorFlow Lite.

## Project Overview

The project aims to classify forest types using spectral data. The dataset consists of **326 instances** and **27 features**, including various spectral bands and prediction error columns.

- **Subject Area:** Biology
- **Associated Tasks:** Classification
- **Data Characteristics:** Multivariate
- **Total Instances:** 326
- **Features:** 27

## Dataset

The dataset includes training and testing files, located in the `data/` folder:
- `training.csv` - for training the neural network model
- `testing.csv` - for evaluating the model's performance

The data was donated on 5/24/2015 and represents spectral data collected over a forested region in Japan. The goal is to map different forest types based on their spectral characteristics.

## Neural Network Model

The neural network model is designed with a small architecture suitable for constrained environments. After training, it is saved in Keras format and then converted to TensorFlow Lite for deployment on the ESP32.

## Repository Structure

- `data/` - Contains the dataset files (training and testing).
- `model/` - Includes the saved Keras model (`forest_model.h5`) and the converted TFLite model (`forest_model.tflite`).
- `scripts/` - Includes Python scripts for data preprocessing, model training, TFLite conversion, and ESP32 deployment.
- `Forest_ESP32/` - Includes Forest_ESP32.ino with the generated header file to run on ESP32.
- `README.md` - Project documentation.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/VedanshMaheshwari/forest-type-mapping-ESP32.git

## Contributing
Feel free to open issues or submit pull requests for improvements.

