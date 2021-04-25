# CorruptionRobustness
For [CS1678](https://people.cs.pitt.edu/~kovashka/cs1678_sp21/), my group explored corruption robustness across different Convolutional Neural Network and Vision Transformer architectures. 

## Corruption Robustness Baselines

View our [Google Colab]() to reproduce our experiments.

| Model | Pretrained on ? | Evaluation Data Set | Top-1 | 
| :---: | :-----------------: | :-----------------: | :---: |
| ResNet50 | ImageNet | Subset of ImageNet-C | 19.63 % |
| SIN (_ResNet50_) | Stylized-ImageNet | Subset of ImageNet-C | 32.31 % |
| ViT_B_16 | ImageNet21K + ImageNet1K | Subset of ImageNet-C | 33.88 % |
| DeiT-base | ImageNet | Subset of ImageNet-C | 47.44 % |
| swin_tiny_patch4_window7 | ImageNet | Subset of ImageNet-C | 37.25 % |

## Shape Bias

View our [Google Colab](https://colab.research.google.com/drive/1gu8XQjtA4lLEF69bT226_eO_67_nIGTu?usp=sharing) to reproduce our experiments. 

| Model | Pretrained on ? | # params | Shape Bias |
|:---:  | :---: | :---: | :----: |
| ResNet50 | ImageNet | 26M | 26.17 % |
| SIN (_ResNet50_) | Stylized-ImageNet | 26M | 76.52 % |
| SIN+IN (_ResNet50_) | Stylized-ImageNet & ImageNet | 26M | 38.70 % |
| ViT_B_16 | ImageNet21K + ImageNet1K | 87M | 41.49 % |
| DeiT-base | ImageNet | 87M | 42.32 % |
| DeiT-tiny | ImageNet | 5M | 29.37 % |
| DeiT-tiny distilled | ImageNet | 6M | 31.06 % |
| DeiT-small | ImageNet | 22M | 38.26 % |

## Analysis

There are two key results to point out from these experiments. First, take note how all of the vision transformer architectures perform better on a subset of ImageNet-C than a vanilla ResNet50 and a ResNet50 trained on Stylized-ImageNet. From this, we decided to see how much shape bias vision transformers have compared to a vanilla ResNet50. Notice how a the DeiT tiny vision transformer achieves a higher shape bias than a vanilla ResNet50, and yet ResNet50 has 5 times as many parameters at the DeiT tiny model. 
