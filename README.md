# CorruptionRobustness
For [CS1678](https://people.cs.pitt.edu/~kovashka/cs1678_sp21/), my group explored corruption robustness across different Convolutional Neural Network and Vision Transformer architectures. 

## Corruption Robustness Baselines

View our [Google Colab]() to reproduce our experiments.

| Model | Pretrained on ? | Evaluation Data Set | Top-1 | 
| :---: | :-----------------: | :-----------------: | :---: |
| ResNet50 | ImageNet | Subset of ImageNet-C | 19.63 % |
| SIN (_ResNet50_) | Stylized-ImageNet | Subset of ImageNet-C | 32.31 % |
| ViT_B_16 | ImageNet21K + ImageNet1K | Subset of ImageNet-C | 33.88 % |
| DeiT_base_patch16 | ImageNet | Subset of ImageNet-C | 47.44 % |
| Swin_tiny_patch4_window7 | ImageNet | Subset of ImageNet-C | 37.25 % |

## Shape Bias

View our [Google Colab](https://colab.research.google.com/drive/1gu8XQjtA4lLEF69bT226_eO_67_nIGTu?usp=sharing) to reproduce our experiments. 

| Model | Pretrained on ? | # params | Shape Bias |
|:---:  | :---: | :---: | :----: |
| ResNet50 | ImageNet | 26M | 26.17 % |
| SIN (_ResNet50_) | Stylized-ImageNet | 26M | 76.52 % |
| SIN+IN (_ResNet50_) | Stylized-ImageNet & ImageNet | 26M | 38.70 % |
| ViT_B_16 | ImageNet21K + ImageNet1K | 87M | 41.49 % |
| deit_base_patch16 | ImageNet | 87M | 42.32 % |
| deit_tiny_patch16_224 | ImageNet | 5M | 29.37 % |
| deit_tiny_distilled_patch16_224 | ImageNet | 6M | 31.06 % |
| deit_small_patch16_224| ImageNet | 22M | 38.26 % |
|

