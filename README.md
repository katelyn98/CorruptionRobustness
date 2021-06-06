# CorruptionRobustness
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/katelyn98/CorruptionRobustness/blob/master/EvaluatingCorruptionsImageNetC.ipynb)

We explored corruption robustness across different Convolutional Neural Networks, Vision Transformer architectures, and the MLP-Mixer. 

## Corruption Robustness Baselines

View this [Google Colab](https://colab.research.google.com/drive/1I_uV1it2JMGAhDgkdQhlY7y0vKLtW-u3#scrollTo=8I_mGA0TW6aT) to reproduce our experiments.

| Model | mCE(_Sev 2_) | mCE(_Sev 5_) |
| :---: |:-----------------: | :---: |
| ResNet50 | 19.63 % | M|
| SIN (_ResNet50_) | 32.31 % |  M|
| ViT_B_16 | 33.88 % | M|
| DeiT-base | 47.44 % |  M|
| swin_tiny_patch4_window7 | 37.25 % |  M|
 
## Shape Bias

View this [Google Colab](https://colab.research.google.com/drive/1gu8XQjtA4lLEF69bT226_eO_67_nIGTu?usp=sharing) to reproduce our experiments. 

| Model | Shape Bias | # params |
|:---:  | :---: | :----: |
| ResNet50 |  26.17 % | 26M |
| SIN (_ResNet50_)  76.52 % |  26M |
| SIN+IN (_ResNet50_) |38.70 % | 26M | 
| ViT_B_16 | 41.49 % | 87M |
| DeiT-base | 42.32 % |87M | 
| DeiT-tiny | 29.37 % |5M | 
| DeiT-tiny distilled | 31.06 % |6M | 
| DeiT-small |38.26 % | 22M | 

## Analysis

Notice how a the DeiT tiny vision transformer achieves a higher shape bias than a vanilla ResNet50, and yet ResNet50 has 5 times as many parameters at the DeiT tiny model. 
