# Figures Gallery  
## Multimodal Pediatric Sleep Stage Classification

This document visually presents **all figures used in the IEEE paper** with correct rendering paths for GitHub.

---

## 1. Framework & Architecture

### Sleep Processing Pipeline
![Sleep Pipeline](./sleep_pipeline.png)

### Model Architectures
![MultiSleepMLP Architecture](./MultiSleepMLP_Architecture.jpg)

![MultiSleepMLP Architecture v2](./MultiSleepMLP_Architecture_v2.jpg)

---

## 2. Signal Preprocessing

### EEG (F4–M1)

**Raw EEG**
![EEG Raw](./EEG-F4-M1%20(raw-data)%20New.png)

**Filtered EEG**
![EEG Filtered](./EEG-F4-M1%20(filtered)%20New.png)

**Standardized EEG**
![EEG Standardized](./EEG-F4-M1%20(Standardized).png)

---

### EOG (ROC–M1)

**Raw EOG**
![EOG Raw](./EOG-ROC-M1%20(raw-data)%20New.png)

**Filtered EOG**
![EOG Filtered](./EOG-ROC-M1%20(filtered)%20New.png)

**Standardized EOG**
![EOG Standardized](./EOG-ROC-M1%20(Standardized).png)

---

## 3. Class Imbalance (SMOTE)

**Before SMOTE**
![SMOTE Before](./smote%20Before.png)

**After SMOTE**
![SMOTE After](./smote%20After.png)

---

## 4. Feature Extraction Visualizations

### Temporal Features
![Temporal Features](./temporal%20features%20Scatter%20plot.png)

### Spectral Features
![Spectral Features](./spectral%20features%20Scatter%20plot.png)

### Normalized PSD Features
![Normalized PSD](./Norm%20PSDs%20features%20Scatter%20plot.png)

### CWT Features

**EEG CWT**
![CWT EEG](./CWT%20EEG%20features%20Scatter%20plot.png)

**EOG CWT**
![CWT EOG](./CWT%20EOG%20features%20Scatter%20plot.png)

### Combined Feature Space
![Feature Extraction](./Scatter%20plot%20feature%20extraction.png)

---

## 5. Classification Results

### Confusion Matrix
![Confusion Matrix](./confusion_matrices_highres.png)

### Additional Outputs
![Output](./out.jpeg)
![Output 2](./output%20(2).png)
![Output 3](./output%20(3).png)
![Output 4](./output%20(4).png)
![Output 5](./output%20(5).png)
![Output 6](./output%20(6).png)

---

## 6. Explainable AI (LIME)

### Global Feature Importance
![LIME Score](./lime-score.png)

### Instance-Level Explanations
![LIME 1](./lime%20(1).png)
![LIME 2](./lime%20(2).png)

---

## 7. Supplementary Visuals

![Supplementary](./kk%20(1).png)
![Supplementary](./kk%20(2).png)

---

## Notes
- All paths are **relative to `/Figures`** and render correctly on GitHub.
- Filenames with spaces are URL-encoded (`%20`) as required.
- Figures correspond exactly to those referenced in the IEEE paper.

