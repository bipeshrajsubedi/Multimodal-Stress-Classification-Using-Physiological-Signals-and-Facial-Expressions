# Multimodal Stress Classification Using Physiological Signals and Facial Expressions

This repository contains code and resources for **stress classification** using the **WorkStress3D dataset**, leveraging both physiological signals and facial expressions with deep and machine learning models.

## Dataset

- **Data Types:** Physiological signals and facial expressions  
- **Classes:** 
  - `0` → Stress-free  
  - `1` → Stressed  
- **Link:** [WorkStress3D Dataset](https://data.mendeley.com/datasets/t93xcwm75r/8)

## Models

### Independent Models
Different models are used depending on the data modality. These models are trained independently and **do not combine outputs**, unlike the fusion approach.  

- **Physiological Data:**  
  - Long Short-Term Memory (LSTM)  
  - Support Vector Machine (SVM)  

- **Facial Expressions Data:**  
  - VGG16 (pre-trained CNN)  
  - Custom CNN  

- **Paper Link:** *(add paper link here)*

### Fusion Approach (Exploratory)  
- **Procedure:**  
  1. Train LSTM on physiological data and VGG16 on facial expression data independently.  
  2. Extract predictions/features from both models.  
  3. Combine these outputs to train a **fusion layer**.  

> Note: The fusion layer uses only the outputs from the pre-trained LSTM and VGG16 models; the original data is not directly fed to the fusion model.

### Paper Link: https://zenodo.org/records/19161171

### Citation

Subedi, B. (2026). Multimodal Stress Classification Using Physiological Signals and Facial Expressions with Machine and Deep Learning Models. Zenodo. https://doi.org/10.5281/zenodo.19161171
