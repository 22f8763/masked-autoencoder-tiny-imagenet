\# Masked Autoencoder on Tiny ImageNet



This project implements a Masked Autoencoder (MAE) from scratch in PyTorch for self-supervised image representation learning.



\## Project Overview

The model masks 75% of image patches and learns to reconstruct the missing regions using an asymmetric Vision Transformer encoder-decoder architecture.



\## Dataset

\- Tiny ImageNet-200

\- Images resized to 224x224



\## Model Details

\- Encoder: ViT-Base (12 layers, 768 hidden dim, 12 heads)

\- Decoder: Lightweight Transformer (12 layers, 384 hidden dim, 6 heads)

\- Patch size: 16x16

\- Mask ratio: 75%



\## Training Setup

\- Epochs: 50

\- Batch size: 64

\- Optimizer: AdamW

\- Scheduler: Cosine Annealing

\- Mixed precision training

\- Gradient clipping

\- Multi-GPU support with DataParallel



\## Results

The model reconstructs general image structure and colors reasonably well, although some fine details remain blurry.



\## Demo

Hugging Face Space: https://huggingface.co/spaces/prospect01/masked-autoencoder



\## Author

Muhammad Basit

