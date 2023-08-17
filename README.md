# TransVCOX

## Introduction

 In this paper, we introduce a Transformer-based deep learning model, TransVCOX , which is built upon the pre-trained VAE and the Transformer encoder. The primary goal of TransVCOX is to leverage large-scale cancer datasets to enhance the robustness of feature representation for individual datasets and to offer a risk-based evaluation model for patient prognosis assessment. Initially, our model undergoes feature transformation using the pre-trained VAE \cite{pretrainvae}. 
Following this transformation, it integrates these features with the original data. Subsequently, deep feature extraction is performed utilizing the Transformer encoder . Ultimately, these features are fed into the Cox model for risk assessment.

![](C:\Users\Administrator\Desktop\proj_TransVCOX\TransVCOX\TransVCOX.png)

## Installations

- Linux (Tested on Ubuntu 18.04)

- NVIDIA GPU (Pretrained on a Tesla A100, Training TransVCOX on a single Nvidia GeForce RTX 3090 Ti)

  ```python
  pip install -r requirements.txt
  ```

## Pre-train VAE

```python
python pretrain_vae/pretrain_vae_run.py
```

## Training

```
python TransVCOX/main.py
```

> ## The pre-trained model will be uploaded after the paper is accepted
