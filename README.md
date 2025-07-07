# Deep Learning for Brain Tumor Detection and Segmentation

An advanced deep learning pipeline for automated detection and segmentation of brain tumors in MRI scans using Convolutional Neural Networks and Meta's Segment Anything Model (SAM).

## Project Overview

This project develops a comprehensive solution for brain tumor analysis by combining:
- **CNN Classification**: Binary classification of MRI scans (tumor vs non-tumor)
- **Segmentation Models**: Precise tumor region delineation
- **SAM Integration**: Automated mask generation using Meta's Segment Anything Model
- **Comparative Analysis**: Evaluation of automated vs manual segmentation approaches

## Methodology

### Dataset
- **MRI Scans**: Comprehensive collection of brain MRI images
- **Ground Truth Labels**: Binary tumor presence annotations
- **Segmentation Masks**: Manually annotated tumor region masks
- **Multi-class Segmentation**: Different tumor region classifications

### Model Architecture

#### 1. Classification Pipeline
- **CNN Architecture**: Custom convolutional neural network for binary classification
- **Input Processing**: Standardized MRI scan preprocessing
- **Output**: Tumor presence probability scores

#### 2. Segmentation Framework
- **Residual U-Net**: Advanced encoder-decoder architecture with residual connections
- **Skip Connections**: Preserved spatial information through network depth
- **Multi-scale Features**: Comprehensive feature extraction at multiple resolutions

### Key Components

#### Encoder Blocks
- Convolutional layers with ReLU activation
- Max pooling for spatial dimension reduction
- Progressive feature map expansion

#### Bottleneck
- Residual double convolution layer
- Feature compression and representation learning

#### Decoder Blocks  
- Upsampling with concatenation of encoder features
- Progressive spatial resolution recovery
- Feature map reduction toward output classes
  
---

## Key Research Questions

1. **Classification Accuracy**: How effectively can CNNs detect tumor presence in brain MRI scans?

2. **Segmentation Precision**: What level of accuracy can Residual U-Net achieve for tumor region segmentation?

3. **Automation Feasibility**: Can automated segmentation replace manual annotation in clinical workflows?
