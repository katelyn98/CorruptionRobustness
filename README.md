# CorruptionRobustness

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13KkwC0Rm469PHI7U429JLeAflWLpirvV?usp=sharing)

We explored corruption robustness across different Convolutional Neural Networks, Vision Transformer architectures, and the MLP-Mixer. 

## Corruption Robustness Baselines

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1I_uV1it2JMGAhDgkdQhlY7y0vKLtW-u3?usp=sharing)

| Model | top-1(%) | mCE (%) |
| :---: |:-----------------: | :---: |
| ResNet50 | 19.63 % | M|
| ViT_B_16 | 33.88 % | M|
| DeiT-base | 47.44 % |  M|
| swin_tiny_patch4_window7 | 37.25 % |  M|
 
## Shape Bias

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1gu8XQjtA4lLEF69bT226_eO_67_nIGTu?usp=sharing)

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
