# 🧪 Breast Tumor Cell Nuclei Segmentation

This repository contains source code for the **KMMS paper**:  
## **Breast Tumor Cell Nuclei Segmentation in Histopathology Images using EfficientUnet++ and Multi-organ Transfer Learning**

📄 **Paper Link**: [http://www.koreascience.or.kr/article/JAKO202125761193585.pdf](http://www.koreascience.or.kr/article/JAKO202125761193585.pdf)

---

### 🧾 Abstract

In recent years, using Deep Learning methods for medical and biomedical image analysis has seen many advancements. In clinical applications, Deep Learning-based approaches for cancer image analysis are key for cancer detection and treatment. However, the scarcity of labeled images makes achieving high accuracy challenging.

Since its introduction in 2015, the U-Net model has received widespread attention due to its ability to produce high accuracy with very few training images. Numerous variants and improvements on U-Net have been proposed since then.

This paper proposes a novel approach that utilizes **U-Net++** with a **pretrained EfficientNet** as the backbone for breast tumor cell nuclei segmentation. It also introduces a **multi-organ transfer learning** strategy to segment nuclei of breast tumor cells. Experiments were conducted on the **MoNuSeg training dataset** and the **Triple Negative Breast Cancer (TNBC) testing dataset**, both of which contain Hematoxylin and Eosin (H&E) stained images.

The proposed **EfficientUnet++** architecture combined with multi-organ transfer learning outperformed other techniques, showing notable accuracy in breast tumor cell nuclei segmentation.

---

### 🧠 Model Architecture

![Model Architecture](https://github.com/tuan-ld/breast-tumor-cell-nuclei-segmentation/blob/main/media-sources/model-architecture.png)

---

### 🧬 Samples of Dataset

![Dataset Samples](https://github.com/tuan-ld/breast-tumor-cell-nuclei-segmentation/blob/main/media-sources/dataset.png)

---

### 🎯 Qualitative Output Results

![Output Masks](https://github.com/tuan-ld/breast-tumor-cell-nuclei-segmentation/blob/main/media-sources/output-predicted-mask-1.png)

---

## 🔁 Reproducibility Guide

Follow the steps below to reproduce the experiment and train the model.

---

### 📁 Repository Structure

```
breast-tumor-cell-nuclei-segmentation/
├── dataset/
│   ├── convert-binary-mask-images/
│   │   └── convert-binary-mask-images.ipynb
│   ├── data-normalization/
│   │   └── pipeline-for-stain-normilized-training-keras.ipynb
├── model/
│   └── train_efficient-unet++_on_monuseg_dataset.ipynb
```

---

### ✅ Step 1: Download the Original Dataset

Download the dataset from the [MoNuSeg Challenge](https://monuseg.grand-challenge.org/) or another relevant source.

> 📌 **Note:** Ensure the folder structure matches what the conversion notebook expects.

---

### 🛠️ Step 2: Convert Binary Mask Images

Convert the original dataset into 2D image-mask pairs.

```bash
cd breast-tumor-cell-nuclei-segmentation/dataset/convert-binary-mask-images
```

Open and run the notebook:

```
convert-binary-mask-images.ipynb
```

---

### 🎨 Step 3: Normalize Stains

Perform stain normalization for consistent training data:

```bash
cd ../data-normalization
```

Open and run the notebook:

```
pipeline-for-stain-normilized-training-keras.ipynb
```

---

### 🚀 Step 4: Train and Evaluate the Model

Train the Efficient-UNet++ model:

```bash
cd ../../model
```

Open and run the notebook:

```
train_efficient-unet++_on_monuseg_dataset.ipynb
```

This will perform training and inference using the preprocessed data.

---

## 📊 Validation Strategy

You can manually split your dataset into training and validation sets:

- **70/30 split** – 70% training, 30% validation  
- **80/20 split** – 80% training, 20% validation

> 🎲 **Note:** Your split may differ slightly from ours due to random selection. This may cause minor performance differences.

---

## 🗂️ Output Artifacts

Running the full pipeline will generate:

- ✅ Stain-normalized training/validation images  
- ✅ Trained EfficientUnet++ model weights  
- ✅ Predicted segmentation masks  
- ✅ Evaluation metrics (Dice, IoU, etc.)  
- ✅ Optional visualizations

---

## 📬 Questions or Issues?

Please feel free to open an [Issue](https://github.com/tuan-ld/breast-tumor-cell-nuclei-segmentation/issues) or start a [Discussion](https://github.com/tuan-ld/breast-tumor-cell-nuclei-segmentation/discussions) for help or collaboration.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).  
You are free to use, modify, and distribute this work with attribution.

---

## 📚 Citation

If you find this code useful in your research, please consider citing:

```bibtex
@article{efficientunet++,
  Author = {T. L. Dinh, S.-G. Kwon, S.-H. Lee, and K.-R. Kwon},
  Title = {Breast Tumor Cell Nuclei Segmentation in Histopathology Images using EfficientUnet++ and Multi-organ Transfer Learning},
  Journal  = {Journal of Korea Multimedia Society},
  Year = {2021}
}
```

---

⭐ If this repository helps your work, don’t forget to star it and share it with the community!
