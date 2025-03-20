
# PyTorch CAPTCHA Recognition

## Overview
PyTorch CAPTCHA Recognition is a project aimed at building and training models for CAPTCHA recognition using the PyTorch framework. This repository contains the necessary code, datasets, and instructions to replicate the experiments and results.

## Features
- Implementation of a Convolutional Neural Network (CNN) for CAPTCHA recognition.
- Utility scripts for generating CAPTCHA images and testing the model.
- Configurable settings for CAPTCHA generation and model training.

## Installation
To get started with, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/shallowManica/pytorch-recognition.git
   cd pytorch-recognition
   ```

2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
### Generating CAPTCHA Images
To generate CAPTCHA images for training, run:
```bash
python captcha_gen.py
```

### Training the Model
To train the model, use the following command:
```bash
python train.py --config configs/config.yaml
```

### Testing the Model
To test the model's accuracy, run:
```bash
python captcha_test.py
```

### Predicting CAPTCHA
For inference, use:
```bash
python captcha_predict.py
```

## Directory Structure
```plaintext
pytorch-recognition/
├── configs/             # Configuration files
├── data/                # Datasets and data loaders
├── models/              # Model definitions
├── notebooks/           # Jupyter notebooks for experiments
├── scripts/             # Utility scripts
├── train.py             # Script to train models
├── inference.py         # Script for inference
├── requirements.txt     # List of dependencies
├── captcha_cnn_model.py # CNN model definition
├── captcha_gen.py       # Script to generate CAPTCHA images
├── captcha_predict.py   # Script for CAPTCHA prediction
├── captcha_test.py      # Script to test the model
├── captcha_setting.py   # CAPTCHA settings
└── README.md            # Project documentation
```
