# 【CCB_GlassDefectDataset】
## 1. Dataset Overview
### 1.1 Background & Purpose
This dataset is designed for surface defect detection of roller washing machine glass covers — a key component affecting product safety, appearance quality, and user experience. During the manufacturing (e.g., tempering, polishing, assembly) and transportation processes of washing machine glass covers, surface defects such as scratches, bubbles, and impurities are prone to occur. These defects not only reduce the product’s aesthetic value but may also lead to structural damage (e.g., glass breakage) during use.
To address the lack of specialized datasets for this specific scenario (existing glass defect datasets mostly target flat glass, optical glass, etc., and do not match the curved structure, texture, and defect characteristics of washing machine glass covers), we independently collected and annotated real-world samples to support the development, training, and evaluation of defect detection models (e.g., CNN, YOLO, Mask R-CNN) in industrial quality inspection scenarios.
### 1.2 Basic Information
Data Source: Real samples collected from a domestic glass product manufacturing factory.​
Sample Quantity: A total of 872 images (The training set contains 741 images, while the validation set includes 131 images).​
Image Specifications:​
Resolution: 5120×5120 pixels.​
Format: JPG.​
Shooting Environment: Controlled factory lighting (5000K natural white light, no glare) + rotational shooting.​
Collection Equipment: Hikvision Industrial CCD Camera + macro lens (10x magnification for micro-defect capture).

## 2. Dataset Structure
The dataset is organized in a hierarchical folder structure for easy access and model loading:
CCB_GlassDefectDataset/
├── images/                # All image files 
│   ├── train/            # Training set sample paths (741 images)
│   ├── val/              # Test set sample paths (131 images)
├── LICENSE                # Dataset license file (CC BY-NC-SA 4.0)
└── README.md              # Dataset description (this document)

## 3. Usage Notes​
The dataset is for non-commercial use only (see LICENSE for details); commercial use requires prior authorization from the authors.​
When using the dataset for academic research, please cite this repository (citation format provided in Section 6).​
For model training, it is recommended to use data augmentation techniques (e.g., rotation, flipping, brightness djustment) to improve model generalization.

## 4. Citation
If you use this dataset in your research, please cite:
@misc{CCB_GlassDefectDataset,
  author = {shaoqilyx},
  title = {Glass Product Cover Surface Defect Dataset},
  year = {2026},
  publisher = {GitHub},
  journal = {GitHub Repository},
  howpublished = {\url{https://github.com/shaoqilyx/CCB_GlassDefectDataset}}
}

## 5. Author & Contact
- Author: shaoqilyx
- Email: 99832201@qq.com