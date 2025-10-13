🌫️ PM25Vision: Air Quality Estimation from Street-Level Images

This project explores the use of machine learning and deep learning techniques to estimate PM₂.₅ air pollution levels directly from street-level images. Using both supervised and self-supervised learning approaches, the goal is to build models that can support scalable, image-based air quality monitoring systems.

📂 Dataset

Dataset: PM25Vision on Kaggle

The PM25Vision dataset pairs Mapillary street images with historical PM₂.₅ measurements from the World Air Quality Index (WAQI).

🖼️ Images: Street-level views within 5 km of air quality stations

🌍 Coverage: 3,000+ stations worldwide

🧮 Samples: ~11,000 cleaned & balanced image–PM₂.₅ pairs

🕓 Time range: 2014–2025

Each sample contains the image, station ID, geolocation, date, PM₂.₅ value, and a discretized AQI label.

🧠 Methods

The project experiments with a mix of supervised CNNs and self-supervised learning methods to predict PM₂.₅:

Supervised Models: ResNet50, EfficientNet-B0, MobileNetV2, VGG16, ViT

Self-Supervised Methods: SimCLR, BYOL, Barlow Twins

Evaluation: Linear probes, fine-tuning, and classical ML heads on frozen features

📊 Results Overview

Supervised baselines achieved solid performance for both regression and classification.

SSL models produced stronger features in low-label settings and improved linear probe performance.

Embedding analysis (t-SNE, UMAP) showed clear separability between air quality categories.

🚀 Future Work

Real-time mobile deployment for urban air monitoring

Multi-pollutant prediction using multimodal inputs

Integration with IoT-based smart city systems
