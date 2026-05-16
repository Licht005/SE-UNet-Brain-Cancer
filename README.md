# SE-UNet: Brain Tumor Classification

A comparative brain tumor classification study featuring a novel **SE-UNet encoder** architecture, evaluated on the Bangladesh Brain Cancer MRI Dataset.

## Overview

This project integrates Squeeze-and-Excitation (SE) blocks into a UNet-style encoder for brain tumor classification, alongside a comparative framework of standard architectures. The SE-UNet was designed to improve channel-wise feature recalibration in medical imaging contexts where subtle spatial patterns carry diagnostic weight.

## Architecture

The SE-UNet encoder introduces the following over a standard UNet baseline:

- Squeeze-and-Excitation blocks for channel attention at each encoder stage
- Batch Normalization throughout
- Fourth encoder block expanded to 512 channels
- Label smoothing during training
- Cosine Annealing learning rate schedule
- Dropout for regularization

## Results

| Metric | SE-UNet |
|--------|---------|
| Accuracy | 99.06% |
| Precision | 99.07% |
| Recall | 99.07% |
| F1 Score | 99.07% |
| AUC | 0.9997 |

## Dataset

[Bangladesh Brain Cancer MRI Dataset]([https://www.kaggle.com/datasets/](https://www.kaggle.com/datasets/orvile/brain-cancer-mri-dataset)) — MRI scans across tumor classes.

## Repository Contents

- `Brain_Cancer__comparative_modelling.ipynb` — full training and evaluation code
- `Brain cancer methodology.pdf` — detailed documentation of the research design and experimental setup

## Stack

Python, PyTorch, Scikit-learn, Matplotlib
