# Transformer-Based Landslide Detection using Cross-Resolution Feature Fusion

### A Deep Learning + Explainable AI Framework for Automatic Landslide Mapping

---

## 📘 Overview

This project presents a **Transformer-based Ensemble U-Net** model with **Cross-Resolution Feature Fusion (CRFF)** for accurate **landslide detection** using multispectral satellite imagery.  
The framework integrates **edge-aware preprocessing**, **attention mechanisms**, and **hybrid loss optimization** to overcome challenges like data imbalance, small-region segmentation, and poor generalization across terrains.

Additionally, the system employs **Explainable AI (Integrated Gradients)** and an **Adaptive Mamdani Fuzzy Logic module** to enhance interpretability and provide physically meaningful risk assessment.

---

## 🧩 Key Features

- **Hybrid CRFF Transformer U-Net** architecture combining convolution and self-attention.  
- **Cross-resolution feature fusion** for multi-scale spatial context.  
- **Coordinate Attention** for terrain-aware feature refinement.  
- **Edge Enhancement Module** preserving slope and boundary precision.  
- **Dice–Tversky hybrid loss** for imbalanced data stability.  
- **Multispectral input fusion** (RGB, NDVI, SWIR1, SWIR2, slope, elevation).  
- **Explainability using Integrated Gradients (IG)** for spectral-band attribution.  
- **Adaptive Fuzzy Logic (Mamdani model)** for risk-based interpretability.

---

## 🗺️ Dataset
- **Data Type:** Multispectral tiles (14-band HDF5 format)  
- **Selected Bands:** RGB, NDVI, SWIR1, SWIR2, slope, elevation  
- **Split:** 70% training, 15% validation, 15% testing  
- **Preprocessing:**  
  - CLAHE (contrast enhancement in LAB space)  
  - NDVI-based vegetation masking  
  - Multi-scale edge fusion (Canny, LoG, Scharr)  
  - Bilateral filtering and unsharp masking  

