# CorruptionRobustness

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13KkwC0Rm469PHI7U429JLeAflWLpirvV?usp=sharing)

We explored corruption robustness across different Convolutional Neural Networks, Vision Transformer architectures, and the MLP-Mixer. 

## Corruption Robustness Baselines

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1I_uV1it2JMGAhDgkdQhlY7y0vKLtW-u3?usp=sharing)

| Model | top-1 (%) | mCE (%) |
| :---: |:-------: | :---: |
| ResNet50 | % | 26M |
| AlexNet | % | M |
| VGG16 | % | M |
| GoogLeNet | % | M |
| MLP-Mixer-b | % | M |
| MLP-Mixer_l | % | M |
| ViT_B_16 |  % | 87M |
| ViT_L_16 |  % | M |
| DeiT-base |  % |87M | 
| DeiT_base_dist | % | M |
| DeiT-tiny |  % |5M | 
| DeiT-tiny_dist | % |6M | 
| DeiT-small | % | 22M |
| DeiT_small_dist | % | M |
| CaiT_S | % | M |
| CaiT_XXS | % | M |
| Swin-T_base | % | M |
| Swin-T_small | % | M |
| Swin-T_large | % | M |
| Swin-T_tiny | % | M |
 
## Shape Bias

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1gu8XQjtA4lLEF69bT226_eO_67_nIGTu?usp=sharing)

| Model | Shape Bias (%) | # params (M) |
|:---:  | :---: | :----: |
| ResNet50 |  26.17 % | 26M |
| AlexNet | % | M |
| VGG16 | % | M |
| GoogLeNet | % | M |
| MLP-Mixer-b | % | M |
| MLP-Mixer_l | % | M |
| ViT_B_16 | 41.49 % | 87M |
| ViT_L_16 |  % | M |
| DeiT-base | 42.32 % |87M | 
| DeiT_base_dist | % | M |
| DeiT-tiny | 29.37 % |5M | 
| DeiT-tiny_dist | 31.06 % |6M | 
| DeiT-small |38.26 % | 22M |
| DeiT_small_dist | % | M |
| CaiT_S | % | M |
| CaiT_XXS | % | M |
| Swin-T_base | % | M |
| Swin-T_small | % | M |
| Swin-T_large | % | M |
| Swin-T_tiny | % | M |


## Analysis

Notice how a the DeiT tiny vision transformer achieves a higher shape bias than a vanilla ResNet50, and yet ResNet50 has 5 times as many parameters at the DeiT tiny model. 
