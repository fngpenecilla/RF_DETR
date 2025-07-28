# RF_DETR
This project focuses on building an object detection system using the RF-DETR (Receptive Field Enhanced Detection Transformer) model. RF-DETR is an advanced object detection model that allows a better detection performance to small or complex objects while maintaining the benefits of end-to-end optimization and simplicity.

Aquarium Dataset from Roboflow
- contains 1,255 high-quality images of marine life
- 8 distinct classes including fish, jellyfish, penguins, puffins, sharks, starfish, and stingrays.
- 1,171 training samples and 84 test samples.
This dataset suits mechanism research for attention because it features diverse aquatic species with varying sizes, colors, textures, and shapes. The visual complexity and diversity of marine environments provide an excellent testbed for comparing how different attention mechanisms handle various visual features like fine details, large-scale patterns, and complex backgrounds

<img width="988" height="768" alt="image" src="https://github.com/user-attachments/assets/136608b4-fc50-49fb-a575-acd5c21b005b" />


# RF-DETR Object Detection Project

This repository contains code for training and evaluating an object detection model using the RF-DETR (Receptive Field Enhanced Detection Transformer) architecture. The project utilizes a custom dataset hosted on Roboflow, training the model, evaluating it with key metrics such as average precision (mAP) and recall, and generating confusion matrices for performance analysis.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Setup](#setup)
- [Usage](#usage)
- [Evaluation](#evaluation)
- [References](#references)

## Prerequisites

Before running the project, ensure you have the following installed:

- Python 3.6 or higher
- GPU-enabled environment (Google Colab or a local environment with CUDA support)
- Roboflow API key for dataset access
- Hugging Face Access Token

## Installation

1. Install the required Python dependencies, ensure you have a working version of nvidia-smi if using local GPU

## Setup

1. Set your HuggingFace token for model downloading
2. Set up your Roboflow API key to access the custom dataset
3. The project uses a custom dataset from Roboflow, which needs to be downloaded and extracted. This dataset will be used to train and evaluate the RF-DETR model. (dataset = version.download("coco")

## Usage

1. Model Definition and Training: The RFDETRBase model is defined and trained on the custom dataset. You can train the model by running the training script.
2. Plot Training and Validation Loss: After training, you can visualize the training and validation loss using matplotlib.
3. After training, you can evaluate the model using Mean Average Precision (mAP) and plot the results.
4. Then, analyze the model's classification performance, a confusion matrix is generated and displayed.

## Evaluation

The model’s evaluation includes:

Average Precision (AP): Measured during training.
Recall: Evaluated across different epochs.
Confusion Matrix: Provides insights into model's classification performance.


## References:
[1]	https://www.youtube.com/watch?v=dvOK-nYtrGI  
[2]	https://pypi.org/project/rfdetr/ 
[3]	https://universe.roboflow.com/microsoft/coco 
[4]	https://medium.com/red-buffer/roboflow-d4e8c4b52515 
[5]	https://www.thecloudgirl.dev/blog/complete-beginners-guide-to-hugging-face-2025
[6] https://rfdetr.roboflow.com/#:~:text=RF-DETR%20is%20a%20real-time%2C%20transformer-based%20object%20detection%20model,COCO%20benchmark%20alongside%20competitive%20performance%20at%20base%20sizes. 
[7] https://github.com/roboflow/rf-detr 
