# CorruptionRobustness
For [CS1678](https://people.cs.pitt.edu/~kovashka/cs1678_sp21/), my group investigated corruption robustness across different Convolutional Neural Networks and Vision Transformer architectures. 

## Corruption Robustness Baselines

View our [Google Colab]() to reproduce our experiments.

| Model | Pretrained on ? | Evaluation Data Set | Top-1 | 
| :---: | :-----------------: | :-----------------: | :---: |
| ResNet50 | ImageNet | Subset of ImageNet-C | 19.63 % |
| SIN (_ResNet50_) | Stylized-ImageNet | Subset of ImageNet-C | 32.31 % |
| ViT_B_16 | ImageNet21K + ImageNet1K | Subset of ImageNet-C | 33.88 % |
| DeiT_base_patch16 | ImageNet | 47.44 % |
| Swin_tiny_patch4_window7 | ImageNet | 37.25 % |

## Shape Bias

View our [Google Colab](https://colab.research.google.com/drive/1gu8XQjtA4lLEF69bT226_eO_67_nIGTu?usp=sharing) to reproduce our experiments. 

| Model | Pretrained on ? | Shape Bias |
|:---:  | :---: | :---: |
| ResNet50 | ImageNet | 26.17 % |
| SIN (_ResNet50_) | Stylized-ImageNet | 76.52 % |
| SIN+IN (_ResNet50_) | Stylized-ImageNet & ImageNet | 38.70 % |
| ViT_B_16 | ImageNet21K + ImageNet1K | 41.49 % |
| DeiT_base_patch16 | ImageNet | 42.32 % |
