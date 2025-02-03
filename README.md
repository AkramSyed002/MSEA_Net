

# UAV-based Weed Segmentation Framework for Precision Agriculture

This repository contains a novel **UAV-based weed segmentation framework** designed for **precision agriculture**. The framework leverages advanced **deep learning techniques** to address common challenges in real-time weed detection, such as complex field conditions, variable lighting, and weed-crop overlap. By improving computational efficiency and segmentation accuracy, this method enables effective **weed management** while reducing herbicide dependency in agricultural settings.

## Key Features:
- **Multi-Scale Attention Fusion (MSAF):** This module captures both fine-grained details and global contextual information, providing enhanced feature representation for better weed segmentation.
- **Edge-Enhanced Bottleneck Attention (EEBA):** By integrating edge-aware information, this module improves the precision of segmenting boundaries, especially in areas with subtle differences between crops and weeds.
- **Lightweight Architecture:** Optimized for deployment on edge devices, enabling real-time weed detection without heavy computational requirements.
- **Robustness Across Diverse Environments:** Evaluated on various publicly available agricultural datasets, the model performs well under conditions with variable lighting, complex backgrounds, and overlapping weed-crop regions.

## Contributions:
1. **Improved segmentation accuracy** using multi-scale attention mechanisms and edge-enhanced features.
2. **Optimized computational efficiency,** making the method feasible for real-time UAV deployment in resource-limited environments.
3. **High generalization** across diverse agricultural environments, supporting scalability and flexibility in real-world applications.
4. **Public dataset evaluations** demonstrating superior performance over state-of-the-art methods (measured by Precision, Recall, F1-score, and mean IoU).

## Note on Code Availability:
The code for this UAV-based weed segmentation framework will be made publicly available once the related paper is published. Stay tuned for updates!

---

## Results Comparison:

We comprehensively evaluate our approach on publicly available datasets, demonstrating superior performance over existing state-of-the-art methods in terms of Precision, Recall, F1-score, and mean IoU. By addressing key limitations of current UAV-based segmentation techniques, our method advances precision weed detection, contributing to more efficient and sustainable agricultural practices.

To support reproducibility and further research, the full MSEA-Net implementation is available on [GitHub](https://github.com/AkramSyed002/MSEA_Net). Additionally, the datasets used for evaluation can be accessed from [CoFly-WeedDB](https://github.com/CoFly-Project/CoFly-WeedDB) and [motion blurred UAV images of sorghum fields](https://data.mendeley.com/datasets/4hh45vkp38/5). We encourage researchers to explore and contribute to the code for agricultural applications.



###  **Comparative Evaluation of MSEA-Net**

| **Model**    | **Mean IoU** | **Precision** | **Recall** | **F1-Score** | **IoU (Bg)** | **IoU (Crop)** | **IoU (Weed)** |
|--------------|--------------|---------------|------------|--------------|--------------|----------------|----------------|
| **MSEA-Net** | **90.35**    | **95.01**     | **93.72**  | **94.36**    | **98.74**    | **84.85**      | **80.98**      |



