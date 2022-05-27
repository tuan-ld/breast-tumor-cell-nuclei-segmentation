# breast-tumor-cell-nuclei-segmentation
This repository contains source code for KMMS paper : 

## Breast Tumor Cell Nuclei Segmentation in Histopathology Images using EfficientUnet++ and Multi-organ Transfer Learning

Paper link: https://www.mdpi.com/2076-3417/12/10/4861

### Abstract
The coronavirus pandemic started in Wuhan, China in December 2019, and put millions of peo-ple in a difficult situation. This fatal virus spread to over 227 countries and the number of infect-ed patients increased to over 400 million cases, causing over 6 million deaths worldwide. Due to the serious consequence of this virus, it is necessary to develop a detection method that can re-spond quickly to prevent the spreading of COVID-19. Using chest X-ray images to detect COVID-19 is one of the promising techniques; however, with a large number of COVID-19 in-fected cases every day, the number of radiologists available to diagnose the chest X-ray images is not sufficient. We must have a computer aid system that helps doctors instantly and automati-cally determine COVID-19 cases. Recently, with the emergence of deep learning methods ap-plied for medical and biomedical uses, using convolutional neural net and transformer applica-tions for chest X-ray images can be a supplement for COVID-19 testing. In this paper, we attempt to classify three types of chest X-ray, which are normal, pneumonia, and COVID-19 using deep learning methods on a customized dataset. We also carry out an experiment on the COVID-19 severity assessment task using a tailored dataset. Five deep learning models were obtained to conduct our experiments: DenseNet121, ResNet50, InceptionNet, Swin Transformer, and Hybrid EfficientNet-DOLG neural networks. The results indicated that chest X-ray and deep learning could be reliable methods for supporting doctors in COVID-19 identification and severity as-sessment tasks.

### Model architecture

![alt text](https://github.com/tuan-ld/covid-19-chest-xray-classification-severity-assessment/blob/main/media/EfficientNet-DOLG.png) 


### Samples of dataset classification task
![alt text](https://github.com/tuan-ld/covid-19-chest-xray-classification-severity-assessment/blob/main/media/covid-classification-dataset.PNG)


### Samples of dataset severity assessment task
![alt text](https://github.com/tuan-ld/covid-19-chest-xray-classification-severity-assessment/blob/main/media/covid-severity-assessment-dataset.PNG)



### Confusion matrix and Training history Classification task
![alt text](https://github.com/tuan-ld/covid-19-chest-xray-classification-severity-assessment/blob/main/media/classification-confusion-matrix-training-history.PNG)


### Confusion matrix and Training history Severity Assessment task
![alt text](https://github.com/tuan-ld/covid-19-chest-xray-classification-severity-assessment/blob/main/media/severity-confusion-matrix-training-history.PNG)

### Citation
If you find this code useful in your research, please consider citing:

    @article{efficientunet++,
	Author = {Le Dinh, T.; Lee, S.-H.; Kwon, S.-G.; Kwon, K.-R.},
	Title = {COVID-19 Chest X-ray Classification and Severity Assessment Using Convolutional and Transformer Neural Networks},
	Journal  = { Applied Sciences},
	Year = {2022}
    }

