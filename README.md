# Fashion-MNIST Clothing Classification with CNN

Fashion-MNIST 데이터셋을 사용해 PyTorch 기반 CNN 이미지 분류 모델을 구현한 프로젝트입니다.  
모델을 직접 학습시키고, 테스트 데이터에서 성능을 평가했습니다.  
예측 결과와 오분류 사례를 확인하며 이미지 분류 모델의 학습 및 평가 과정을 경험했습니다.

해당 프로젝트는 Google Colab에서 개발 및 실행된 후, GitHub에 업로드되었습니다.

## Overview

This project implements a Convolutional Neural Network (CNN) to classify clothing images into 10 categories using the Fashion-MNIST dataset.

The project covers:
- Loading and exploring the dataset
- Building and training a CNN model
- Evaluating the model on test data
- Visualizing predictions and inspecting misclassified images

## Tech Stack

- Python
- PyTorch
- Torchvision
- Matplotlib
- Google Colab

## Dataset

[Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist)

- 60,000 training images and 10,000 test images
- 28 × 28 grayscale images
- 10 clothing categories

The dataset is downloaded automatically using Torchvision.

## Model Architecture

| Layer | Configuration |
|---|---|
| Input | 1 × 28 × 28 |
| Convolution | 1 → 16 channels, 3 × 3 kernel, padding 1 |
| Activation | ReLU |
| Max Pooling | 2 × 2 |
| Flatten | 3,136 features |
| Fully Connected | 3,136 → 128 |
| Activation | ReLU |
| Output | 128 → 10 |

## Training Configuration

| Setting | Value |
|---|---|
| Optimizer | Adam |
| Learning Rate | 0.001 |
| Loss Function | CrossEntropyLoss |
| Batch Size | 64 |
| Epochs | 5 |
| Random Seed | 2026 |

## Results

| Metric | Result |
|---|---:|
| Test Accuracy | **90.60%** |
| Correct Predictions | 9,060 / 10,000 |

The result is from the recorded notebook execution. Performance may vary between runs.

## Prediction and Error Analysis

The notebook includes:
- Single-image prediction
- Visualization of predictions on multiple test images
- A bar chart comparing correct and incorrect predictions
- Inspection of up to 10 misclassified images

Some visually similar clothing categories were confused, such as shirts and T-shirts, or coats and pullovers.

## Development Workflow

The project was developed and executed in Google Colab, and the notebook was subsequently uploaded to GitHub for sharing and version control.


## How to Run

1. Open the notebook from this repository in Google Colab.
2. Run the notebook cells in order.
3. The Fashion-MNIST dataset will be downloaded automatically through Torchvision.

## Environment

Recorded execution environment:

- PyTorch: 2.11.0+cpu
- Torchvision: 0.26.0+cpu
- GPU: Not available
