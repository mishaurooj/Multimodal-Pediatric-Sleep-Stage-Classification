# Multimodal Pediatric Sleep Stage Classification

Official repository for the research article:

**An Ensemble Learning Framework for Pediatric Sleep Stage Classification Using Multimodal EEG–EOG Signals, Multi-Domain Features, and LIME-Based Explainability**

(See full paper for methodological and experimental details.)

---

## Overview
This repository contains the complete implementation, figures, tables, and results for a multimodal ensemble framework for pediatric sleep stage classification using EEG and EOG signals. The framework integrates robust preprocessing, multi-domain feature extraction, ensemble learning, and explainable AI (LIME).

Key highlights:
- Dataset: Nationwide Children’s Hospital Sleep Data Bank (NCHSDB)
- Modalities: EEG (F4–M1), EOG (ROC–M1)
- Features: 137 handcrafted (time, frequency, CWT, PSD)
- Best model: Ensemble Bagging Decision Tree (EBDT2)
- Accuracy: 99.96%, Weighted F1-score: 99.99%

---

## Repository Structure
- Code/: Source code for preprocessing, feature extraction, training, and evaluation
- Dataset/: Dataset access instructions (raw PSG data not redistributed)
- Figures/: All figures used in the paper
- Results/: Confusion matrices and result tables
- LICENSE: Apache 2.0
- README.md: This file

---

## Figures and Tables
All figures and tables reported in the paper are provided in the Figures/ and Results/ directories, including:
- Proposed methodology pipeline
- EEG/EOG raw, filtered, and standardized epochs
- SMOTE class balancing visualization
- Multi-domain feature scatter plots
- Confusion matrices of all models
- LIME feature importance plots
- Comparative tables with literature, runtime, error rates, and performance metrics

---

## Dataset
- Source: NSRR / PhysioNet (NCHSDB)
- Pediatric PSG recordings (≤10 years)
- Sampling rate: 256 Hz
- Sleep stages: Wake, N1, N2, N3, REM

Due to licensing restrictions, raw data are not included. Users must request access from NSRR.

---

## Explainable AI
LIME is used to provide local, model-agnostic explanations for ensemble predictions, highlighting the most influential EEG/EOG features contributing to each sleep-stage decision.

---

## Citation
If you use this repository, please cite:

@article{PediatricSleep2026,
  title={An Ensemble Learning Framework for Pediatric Sleep Stage Classification Using Multimodal EEG--EOG Signals, Multi-Domain Features, and LIME-Based Explainability},
  author={Khan, Hareem and Alkhrijah, Yazeed and Khan, Misha Urooj and Suleman, Ahmad and Faiz, Muhammad Abdullah Husnain Ali and Alawad, Mohamad A. and Kaleem, Zeeshan},
  journal={IEEE Access},
  year={2026}
}

---

## License
Apache License 2.0

---

## Acknowledgment
This work is supported by the Deanship of Scientific Research at Imam Mohammad Ibn Saud Islamic University (IMSIU), Grant No. IMSIU-DDRSP2504.
"""
