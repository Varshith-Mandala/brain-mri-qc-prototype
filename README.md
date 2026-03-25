# 🧠 Brain MRI QC Prototype (INCF Proposal)

## 📌 Overview
This project implements a lightweight prototype for automated quality control (QC) in brain MRI scans.  
It demonstrates how deep learning and simple rule-based scoring can be combined to assess MRI slice quality.

---

## 🚀 Key Features
- Load and process MRI data in NIfTI format (.nii)
- Convert 3D MRI volumes into 2D slices
- Generate labels using segmentation masks
- Train a CNN (ResNet18) for slice classification
- Implement a QC scoring function based on brightness and noise
- Identify and visualize low-quality MRI slices

---

## 🧠 Pipeline

1. Load MRI (.nii) files  
2. Extract 2D slices from 3D volumes  
3. Label slices using segmentation masks  
4. Apply preprocessing (normalization, resizing)  
5. Train a CNN classifier  
6. Compute QC scores for each slice  
7. Visualize good vs bad quality slices  

---

## 📊 Prototype Results

- Validation Accuracy: ~70%  
- Demonstrates that meaningful patterns can be learned from MRI slices  
- QC scoring successfully identifies low-quality slices  

---

## ⚠️ Limitations

- Trained on a very small dataset (single patient)  
- Slice-level labels are coarse  
- Not suitable for clinical use  

---

## 🔮 Future Work

- Multi-patient dataset integration  
- ROI-based learning  
- 3D CNN models  
- Integration into QC-Studio pipeline  

---

## 🛠 Tech Stack

- Python  
- NumPy  
- OpenCV  
- PyTorch  
- NiBabel  
- Matplotlib  
- Scikit-learn  

---

## 🎯 Purpose

This prototype validates the feasibility of integrating automated quality control mechanisms into neuroimaging workflows,  
as part of a proposal for the International Neuroinformatics Coordinating Facility (INCF).

---

## 📂 Sample Outputs

- Good quality MRI slice  
- Low-quality MRI slice  
- Model predictions  

---

## 📌 Note

This is a proof-of-concept prototype, not a production system.
