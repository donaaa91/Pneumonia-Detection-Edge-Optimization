# 🫁 4MB Radiologist: Medical Edge AI Optimization

This project demonstrates the optimization of a deep learning model for pneumonia detection, specifically designed for deployment on $20 edge devices in rural clinics with no internet.

## 📊 Performance Impact
| Metric | Baseline (ResNet-50) | Optimized (MobileNet + INT8) | Change |
| :--- | :--- | :--- | :--- |
| **Model Size** | 89.99 MB | 4.23 MB | **21.3x Reduction** |
| **Latency (CPU)** | ~300 ms | 42 ms | **7x Speedup** |
| **Connectivity** | Cloud Required | **Fully Offline** | **Edge Ready** |

## 🛠️ Techniques Applied
* **Knowledge Distillation:** Mimicking ResNet-50 features into a MobileNetV3 architecture.
* **Dynamic INT8 Quantization:** Slashing memory footprint by converting weights from FP32 to INT8.
* **Explainable AI (Grad-CAM):** Visual validation to ensure the model focuses on pulmonary pathology.

## 🚀 How to Use
1. Open `Edge_Optimization_Main.ipynb` in Google Colab.
2. Ensure you have your Kaggle API key to pull the NIH/Kaggle Chest X-ray dataset.
3. The notebook will guide you through the training, distillation, and quantization steps.
