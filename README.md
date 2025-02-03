

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

| **Backbone CNN**   | **Model**    | **Mean IoU** | **Precision** | **Recall** | **F1-Score** | **IoU (Bg)** | **IoU (Crop)** | **IoU (Weed)** |
|--------------------|--------------|--------------|---------------|------------|--------------|--------------|----------------|----------------|
| **VGG16**          | **SegNet**   | 79.12        | 83.52         | 93.23      | 87.86        | 97.62        | 74.69          | 65.05          |
|                    | **UNet**     | 86.15        | 92.23         | 92.58      | 92.40        | 98.60        | 82.83          | 77.01          |
|                    | **DeepLabV3+**| 71.25       | 73.71         | 95.65      | 81.94        | 96.30        | 68.52          | 48.93          |
| **ResNet50**       | **SegNet**   | 82.04        | 88.40         | 91.26      | 89.79        | 98.14        | 78.22          | 69.75          |
|                    | **UNet**     | 84.52        | 93.23         | 89.71      | 91.38        | 98.49        | 81.09          | 74.02          |
|                    | **DeepLabV3+**| 69.43       | 71.77         | 96.00      | 80.21        | 95.96        | 69.64          | 42.70          |
| **DenseNet121**    | **SegNet**   | 81.64        | 87.56         | 91.69      | 89.54        | 98.08        | 77.67          | 69.19          |
|                    | **UNet**     | 84.46        | 92.33         | 90.40      | 91.34        | 98.52        | 81.14          | 73.73          |
|                    | **DeepLabV3+**| 68.50       | 70.94         | 95.90      | 79.00        | 95.81        | 72.27          | 37.41          |
| **EfficientNetB0** | **SegNet**   | 79.90        | 86.44         | 90.46      | 88.37        | 97.87        | 75.88          | 65.96          |
|                    | **UNet**     | 85.34        | 93.62         | 90.27      | 91.88        | 98.60        | 82.59          | 74.82          |
|                    | **DeepLabV3+**| 71.86       | 74.39         | 95.66      | 82.16        | 96.68        | 72.06          | 68.30          |
| **MobileNetV2**    | **SegNet**   | 78.96        | 86.30         | 89.21      | 87.71        | 97.84        | 74.70          | 64.33          |
|                    | **UNet**     | 83.27        | 87.06         | 87.47      | 87.24        | 84.02        | 47.21          | 08.05          |
|                    | **DeepLabV3+**| 64.55       | 68.81         | 88.23      | 76.22        | 95.48        | 60.38          | 37.78          |
| **MSEA-Net**       | **MSEA-Net** | **87.42**    | **93.54**     | **92.61**  | **93.07**    | **99.19**    | **84.00**      | **79.08**      |



