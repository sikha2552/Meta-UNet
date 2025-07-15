# Meta-UNet
Meta-UNet: Enhancing Skin-Lesion Segmentation with Multimodal Feature Integration and Uncertainty Estimation
Meta-UNet is a modified U-Net architecture designed to improve the accuracy and confidence of skin lesion segmentation by integrating lesion-specific metadata. It also incorporates a Bayesian framework using Monte Carlo Dropout (MCD) for uncertainty estimation. This repository contains the implementation, pretrained models, and experimental setup described in the paper ..

**Purpose**
Medical image segmentation plays a crucial role in diagnostic pipelines. This study investigates the integration of lesion-specific metadata with image data to enhance segmentation accuracy and reduce predictive uncertainty.

**Methods**
The standard U-Net architecture was modified to incorporate lesion-specific metadata (Meta-UNet). Various integration strategies, including addition, weighted addition, and embedding layers, were evaluated. Additionally, a
Bayesian Meta-UNet with Monte Carlo Dropout (MCD) was developed to assess the impact of metadata integration on model uncertainty. Uncertainty was quantified using measures such as Confidence Maps, Entropy, Mutual Information, and
Expected Pairwise Kullback-Leibler divergence (EPKL). An aggregation strategy was also introduced to provide a single comprehensive uncertainty score per image.

**Results**
Meta-UNet outperformed standard U-Net across PH2, ISIC 2018, and HAM10000 datasets. On PH2, it achieved 84.64% accuracy and 90.62% Intersection over Union (IoU), compared to 83.36% and 89.19%. On ISIC 2018, U-Net scored
71.02 ± 6.69 IoU and 79.89 ± 5.09 Dice. On HAM10000, Meta-UNet achieved 88.66 ± 6.09 IoU and 93.42 ± 5.19 Dice. Meta-UNet reduced uncertainty (e.g., 0.149 vs. 0.1745), highlighting the benefit of metadata integration in improving
segmentation accuracy and model confidence.

**Conclusion**
Integrating lesion-specific metadata into the U-Net architecture significantly improves segmentation accuracy and reduces predictive uncertainty. The inclusion of metadata enhances model confidence and reliability, underscoring its
potential to strengthen diagnostic segmentation pipelines.


## 🧠 Motivation

Medical image segmentation models often lack uncertainty quantification and ignore rich metadata like lesion type or dermoscopic features. Meta-UNet addresses these limitations by:

- Embedding metadata into the bottleneck of the U-Net.
- Reducing segmentation uncertainty with Bayesian inference.
- Providing better model confidence and robustness in clinical scenarios.

---

## 🛠️ Features

- ✅ Metadata-aware U-Net for improved segmentation.
- ✅ Embedding-based feature fusion.
- ✅ Monte Carlo Dropout for Bayesian uncertainty quantification.
- ✅ Support for PH2, ISIC-2018, and HAM10000 datasets.
<img width="4225" height="3460" alt="arch" src="https://github.com/user-attachments/assets/7bce2cf2-5acc-45b7-8ccd-2c8c75d77470" />
<img width="1280" height="720" alt="1" src="https://github.com/user-attachments/assets/197cda62-f41b-402a-9371-b93e517f0359" />
<img width="1280" height="720" alt="2" src="https://github.com/user-attachments/assets/4830ade6-fcc9-4811-822a-9b80e28a2032" />


📚 Citation
If you find this work useful, please cite: Update soon

🤝 Acknowledgements
This work was supported by the MIT-Spain MISTI Program. We thank the ISIC, PH2, and HAM10000 contributors for their open datasets.

📬 Contact
For questions or collaborations, reach out to:

Sikha O K – sikha.okkath@upf.edu
