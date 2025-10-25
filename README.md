\# ResNet Image Forgery Detection



\## Overview

This project uses a custom-built \*\*ResNet-50\*\* model to classify images as \*\*real\*\* or \*\*AI-generated/edited (fake)\*\*.  

It demonstrates image authenticity detection — a trending topic in AI research.



\## Dataset

\- Dataset: RVF10K (Real vs Fake Images)  

\- Train, Validation, Test split used for model training and evaluation.  

\- Small sample data from Kaggle “AI-generated images” datasets used.



\## Model Architecture

\- Custom ResNet-50 implemented from scratch using TensorFlow/Keras.  

\- Residual blocks with Conv2D, BatchNormalization, Activation layers.  

\- Output: binary classification (real vs fake) using sigmoid activation.  



\## Training

\- Optimizer: Adam  

\- Loss: Binary Crossentropy  

\- Epochs: 8 (for demo / quick run)  

\- Steps per epoch reduced for faster training in Colab.  



\## Results

| Metric | Value |

|--------|-------|

| Test Accuracy | 0.7315 |

| Test Loss     | 0.5678 |

| F1-score (fake) | 0.71 |

| F1-score (real) | 0.75 |



\## How to Use

1\. Open the notebook in Colab or locally.  

2\. Mount Google Drive (if using Colab) to save/load models.  

3\. Run training or inference cells.  

4\. The trained model is saved at: `models/resnet50\_quick\_run.h5`  



\## Notes

\- Model weights can be large (>100MB) — use Git LFS if pushing `.h5` files to GitHub.  

\- This project is suitable for showcasing ML skills in image classification and ResNet implementation.



