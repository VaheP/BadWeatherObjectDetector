# Object Detection in Adverse Weather Conditions

This repository contains the implementation of a project focused on enhancing object detection under adverse weather conditions, such as fog, rain, snow, and sandstorms. The project leverages transfer learning using YOLOv11, dataset augmentation, and synthetic haze generation techniques to improve detection accuracy in challenging scenarios.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Acknowledgments](#acknowledgments)

## Overview
This project tackles the issue of degraded object detection performance in adverse weather. Using YOLOv11 and synthetic data augmentation, we demonstrate significant accuracy improvements for object detection tasks.

Key highlights:
- Training and evaluation using the DAWN dataset.
- Synthetic haze generation using depth prediction and atmospheric scattering models.
- Improved accuracy on validation and test datasets with augmented training data.

## Features
- **Dataset Preprocessing**: Automated cleaning and augmentation using [Roboflow](https://roboflow.com).
- **Synthetic Haze Generation**: Implementation of Tran Le Anh's haze synthesis model to create realistic fog effects.
- **Object Detection Model**: Fine-tuned YOLOv11 with customized hyperparameters.
- **Evaluation Metrics**: IoU (Intersection over Union) and mAP (Mean Average Precision) for comprehensive model assessment.

## Dataset
The project mainly uses the DAWN dataset, which contains images labeled for object detection under adverse weather conditions. Additional synthetic data is generated using haze synthesis techniques to augment the dataset.

## Installation
Clone the repository and install the required dependencies:
```bash
git clone https://github.com/VaheP/BadWeatherObjectDetector
cd BadWeatherObjectDetector
```
### To install the project requirements

```bash
pip install -r requirements.txt
```
## Acknowledgements
This project incorporates code and methodologies from Tran Le Anh’s haze synthesis model. You can find the original work here: https://towardsdatascience.com/synthesize-hazy-foggy-image-using-monodepth-and-atmospheric-scattering-model-9850c721b74e