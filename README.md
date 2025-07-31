# Dual-Branch EfficientNet Architecture for ACL Tear Detection in Knee MRI

## Overview

This project presents a deep learning-based approach to automatically detect Anterior Cruciate Ligament (ACL) tears in knee MRI scans using a dual-branch EfficientNet architecture. By leveraging both sagittal and coronal views of MRI sequences, the model enhances detection accuracy through multimodal feature learning.

## Objectives

- Develop a robust CNN architecture using EfficientNet for ACL tear detection.
- Fuse features from sagittal and coronal MRI sequences via a dual-branch network.
- Improve diagnostic accuracy compared to single-view models.

## Dataset

- **MRNet Dataset** from Stanford (ACL tear classification task)
- Contains T1, T2, and PDFS sequences from knee MRIs in sagittal, coronal, and axial planes.

## Methodology

- **Preprocessing**:
  - Slice selection and normalization
  - Resize to standard resolution
- **Model Design**:
  - Two EfficientNet branches (one for each view)
  - Feature concatenation and classification head
- **Training**:
  - Cross-entropy loss
  - Adam optimizer
  - Evaluation using accuracy, sensitivity, and AUC

## Results

- The dual-branch model outperformed single-branch models on validation accuracy and AUC.
- Demonstrated clinical potential for automated ACL tear screening.

## Tools & Libraries

- Python, PyTorch, NumPy, OpenCV
- EfficientNet-PyTorch
- scikit-learn, matplotlib


## Acknowledgements

Thanks to the Stanford ML Group for the MRNet dataset and related resources.
