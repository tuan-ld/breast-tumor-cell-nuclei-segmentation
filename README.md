# breast-tumor-cell-nuclei-segmentation
This repository contains source code for KMMS paper : 

## Breast Tumor Cell Nuclei Segmentation in Histopathology Images using EfficientUnet++ and Multi-organ Transfer Learning

Paper link: http://www.koreascience.or.kr/article/JAKO202125761193585.pdf

In recent years, using Deep Learning methods to apply for medical and biomedical image analysis has seen many advancements. In clinical, using Deep Learning-based approaches for cancer image analysis is one of the key applications for cancer detection and treatment. However, the scarcity and shortage of labeling images make the task of cancer detection and analysis difficult to reach high accuracy. In 2015, the Unet model was introduced and gained much attention from researchers in the field. The success of Unet model is the ability to produce high accuracy with very few input images. Since the development of Unet, there are many variants and modifications of Unet related architecture. This paper proposes a new approach of using Unet++ with pretrained EfficientNet as backbone architecture for breast tumor cell nuclei segmentation and uses the multi-organ transfer learning approach to segment nuclei of breast tumor cells. We attempt to experiment and evaluate the performance of the network on the MonuSeg training dataset and Triple Negative Breast Cancer (TNBC) testing dataset, both are Hematoxylin and Eosin (H & E)-stained images. The results have shown that EfficientUnet++ architecture and the multi-organ transfer learning approach had outperformed other techniques and produced notable accuracy for breast tumor cell nuclei segmentation

### Model architecture

![alt text](https://github.com/tuan-ld/breast-tumor-cell-nuclei-segmentation/blob/main/media-sources/model-architecture.png)


### Samples of dataset
![alt text](https://github.com/tuan-ld/breast-tumor-cell-nuclei-segmentation/blob/main/media-sources/dataset.png)


### Qualitative output results
![alt text](https://github.com/tuan-ld/breast-tumor-cell-nuclei-segmentation/blob/main/media-sources/output-predicted-mask-1.png)
