# CorruptionRobustness
For CS1678 (Intro to Deep Learning), my group investigated corruption robustness across different architectures including Convolutional Neural Networks and Vision Transformers. 

## Shape Bias

View our [Google Colab](https://colab.research.google.com/drive/1gu8XQjtA4lLEF69bT226_eO_67_nIGTu?usp=sharing) to reproduce our experiments. 

| Model | Pretrained Data Set | Shape Bias |
|:---:  | :---: | :---: |
| ResNet50 | ImageNet | 26.17 % |
| SIN (_ResNet50_) | Stylized-ImageNet | 76.52 % |
| SIN+IN (_ResNet50_) | Stylized-ImageNet & ImageNet | 38.70 % |
| ViT_B_16 | ImageNet21K + ImageNet1K | 41.49 % |
| DeiT_base_patch16 | ImageNet | 42.32 % |
