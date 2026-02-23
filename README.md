# Robustness Analysis of PointConv: Deep Convolutional Networks on 3D Point Clouds

## Introduction
This project is based on the CVPR 2019 paper "PointConv: Deep Convolutional Networks on 3D Point Clouds". You can find the original arXiv version here.
This project was conducted as part of the Deep Learning course by MVA/CentraleSupélec. The primary aim of this project is to study the robustness of the PointConv architecture.

## Usage
Our robustness analysis is available in the Jupyter Notebook titled DeepLearning.ipynb.

### Environment
Platform: Google Colab
GPU: T4 (recommended)
PyTorch: We have updated the authors' original code to be compatible with the latest versions of PyTorch.

### Note for Teachers
It is sufficient to run the notebook we provided you. It contains a command to clone this repository along with the necessary weights. Detailed explanations for each step are included within the cells.

### Training & Evaluation
We have provided the checkpoint for our training. However, if you wish to train or evaluate the model yourself, use the following commands:

To train the model:

Bash
python train_cls_conv.py --model pointconv_modelnet40 --normal --epoch 10 --batchsize 64

To evaluate the model:

Bash
python eval_cls_conv.py --checkpoint ./checkpoints/checkpoint.pth --normal --batchsize 64

### Dataset
We downloaded the dataset from: chenxaoyu/modelnet-normal-resampled. Further details regarding the dataset setup are provided within the notebook.

## License
This repository is released under MIT License (see LICENSE file for details).



