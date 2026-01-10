
---

## 🧠 Dataset Description

- **Dataset:** Nationwide Children’s Hospital Sleep Databank (NCHSDB)
- **Subjects:** Pediatric patients (≤ 10 years)
- **Total PSG Studies:** 3,673
- **Sampling Frequency:** 256 Hz
- **Epoch Length:** 30 seconds (AASM standard)
- **Sleep Stages:** Wake, N1, N2, N3, REM
- **Signals Used:**  
  - EEG: F4–M1  
  - EOG: ROC–M1  

⚠️ *Raw PSG data cannot be redistributed. Access is available via NSRR / PhysioNet.*

---

## 🔬 Methodology Overview

<p align="center">
  <img src="Figures/sleep_pipeline.png" width="750">
</p>

**Pipeline Stages**
1. Multimodal channel selection (EEG + EOG)
2. FIR band-pass filtering
3. AASM-compliant epoch segmentation
4. Signal standardization
5. SMOTE-based class balancing
6. Multi-domain feature extraction
7. Ensemble learning
8. Explainable AI (LIME)

---

## 🧪 Signal Preprocessing Visualization

### EEG (F4–M1)
| Raw | Filtered | Standardized |
|-----|----------|--------------|
| ![](Figures/EEG-F4-M1%20(raw-data)%20New.png) | ![](Figures/EEG-F4-M1%20(filtered)%20New.png) | ![](Figures/EEG-F4-M1%20(Standardized).png) |

### EOG (ROC–M1)
| Raw | Filtered | Standardized |
|-----|----------|--------------|
| ![](Figures/EOG-ROC-M1%20(raw-data)%20New.png) | ![](Figures/EOG-ROC-M1%20(filtered)%20New.png) | ![](Figures/EOG-ROC-M1%20(Standardized).png) |

---

## ⚖️ Class Imbalance Handling (SMOTE)

<p align="center">
  <img src="Figures/smote%20Before.png" width="360">
  <img src="Figures/smote%20After.png" width="360">
</p>

SMOTE significantly improves minority N1 stage representation, enabling balanced model learning.

---

## 🧩 Feature Extraction (137 Features)

<p align="center">
  <img src="Figures/temporal%20features%20Scatter%20plot.png" width="700">
</p>

- **Time Domain:** 98 features  
- **Frequency Domain:** 12 features  
- **CWT Features:** 9 features  
- **PSD Features:** 18 features  

### Feature Visualizations
- Temporal Features  
- Spectral Features  
- Normalized PSD Features  
- CWT EEG & EOG Features  

(All figures available in `/Figures`)

---

## 🧠 Classification Models Evaluated

- Logistic Regression  
- Quadratic SVM  
- Subspace k-NN  
- Medium Neural Network  
- Random Forest  
- XGBoost  
- Voting Classifier  
- **EBDT v1**  
- **EBDT v2 (Proposed)**  
- Perceptron  

---

## 🏆 Performance Summary (From Paper)

| Model | Accuracy (%) | Weighted F1 (%) |
|------|-------------|-----------------|
| Quadratic SVM | 82.64 | 83.00 |
| Random Forest | 87.64 | 87.75 |
| XGBoost | 88.89 | 88.99 |
| EBDT v1 | 90.21 | 90.00 |
| **EBDT v2 (Proposed)** | **99.96** | **99.99** |

---

## 📊 Confusion Matrix

<p align="center">
  <img src="Figures/confusion_matrices_highres.png" width="720">
</p>

---

## 🔍 Explainable AI (LIME)

<p align="center">
  <img src="Figures/lime-score.png" width="720">
</p>

LIME reveals entropy, spectral distribution, and PSD features as dominant contributors to sleep stage decisions.

---

## ⚙️ Edge Deployment Analysis

| Feature Config | Accuracy (%) | Latency (ms) | Memory (MB) |
|---------------|-------------|--------------|-------------|
| Full Features | 99.96 | 42 | 18.6 |
| Feature Selection | 96.30 | 34 | 12.4 |
| PCA Reduced | 97.90 | 28 | 9.8 |

---

## 📜 License

This project is licensed under the **Apache License 2.0** – free for academic and commercial use with attribution.

---

## 📌 Citation

```bibtex
@article{Khan2026EEL,
  title={Explainable Ensemble Learning on Multimodal Biosignals for Pediatric Sleep Stage Classification},
  journal={IEEE Transactions on Biomedical and Health Informatics},
  year={2026}
}
