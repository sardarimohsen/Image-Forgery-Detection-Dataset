# Hybrid-Image-Forgery-Detection


Official repository for the **HDBK** (Hybrid Deep, Block, and Keypoint) framework and a centralized hub for image forgery detection benchmarks[cite: 1]. This project provides the implementation and datasets for robust detection and pixel-level localization of copy-move manipulations[cite: 1].

## 📄 Overview
The HDBK model addresses the limitations of traditional forensic methods by integrating a triple-architecture deep learning ensemble with Genetic Algorithm (GA) optimization and keypoint-based descriptors[cite: 1]. It is designed to be resilient against geometric transformations such as scaling and rotation, as well as post-processing attacks like blurring and noise[cite: 1].

### Key Features
*   **Triple-Architecture Ensemble**: Leverages VGG16, MobileNet, and EfficientNetB0 for high-accuracy image-level detection[cite: 1].
*   **Genetic Algorithm Optimization**: Uses GA to optimize block-matching processes, significantly reducing false positives in complex regions[cite: 1].
*   **Pixel-Level Localization**: Employs SIFT, SURF, and FAST descriptors for precise forensic mask generation[cite: 1].
*   **High Performance**: Achieved **97.34% accuracy** and an **87.17% IoU** on the CoMoFoD benchmark[cite: 1].

---

## 📊 Datasets
This repository includes data and benchmarks for the following industry-standard forensic datasets used in our research[cite: 1]:

| Dataset | Description | Key Focus |
| :--- | :--- | :--- |
| **CoMoFoD** | 10,000 images ($512\times512$)[cite: 1] | Post-processing attacks (Blur, Noise, JPEG)[cite: 1] |
| **MICC-2000** | 2,000 images (various sizes)[cite: 1] | Geometric transformations (Scale/Rotation)[cite: 1] |
| **COVERAGE** | 100 original/forged pairs | Similar object copy-move detection |
| **CASIA** | V1 and V2 benchmarks | Splicing and copy-move forgery |
| **GRIP** | $768\times1024$ high-res images[cite: 1] | High-precision pixel-level localization[cite: 1] |

---

## 📚 Publications
If you use this dataset or code in your research, please cite the following papers:

1.  **A hybrid model for image forgery detection using deep learning with block and keypoint methods**  
    *Scientific Reports*, 2026.[cite: 1]
2.  **Copy-move forgery detection and localization using deep learning**  
    *International Journal of Pattern Recognition and Artificial Intelligence*.
3.  **An optimal hybrid method to detect copy-move forgery**  
    *Journal of AI and Data Mining*.
4.  **A survey on deep learning-based image forgery detection**  
    *Pattern Recognition*, 2023.
5.  **Deep learning framework to extract anatomy for mosquito image classification**  
    *Scientific Reports*.

---

## 🛠️ Installation & Usage

### Requirements
*   Python 3.8+
*   TensorFlow / Keras[cite: 1]
*   OpenCV (for SIFT/SURF extraction)[cite: 1]
*   NumPy & Matplotlib

### Quick Start
```bash
# Clone the repository
git clone https://github.com/your-username/image-forgery-detection-dataset.git

# Install dependencies
pip install -r requirements.txt

# Run the HDBK detection script
python main_hdbk_detection.py --input ./dataset/test_image.png
```

---

## 📈 Performance Benchmarks (HDBK)
Results obtained on the **CoMoFoD** dataset[cite: 1]:
*   **Accuracy**: 97.34%[cite: 1]
*   **Precision**: 92.04%[cite: 1]
*   **Recall**: 91.72%[cite: 1]
*   **F1-Score**: 91.85%[cite: 1]
*   **IoU**: 87.17%[cite: 1]

---

## ⚖️ License
This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License**[cite: 1]. For commercial use, please contact the authors.

---
**Contact**: For questions regarding the JAICT journal or this research, please open an issue or contact the corresponding author at Meybod University.
