# Generation and Price Optimization of Fashion Content using DCGAN

## 📌 Project Overview

This project explores the application of Deep Convolutional Generative Adversarial Networks (DCGANs) to automatically generate realistic fashion images and applies machine learning techniques to optimize pricing strategies based on visual content. By leveraging GANs and predictive modeling, we aim to support creative design workflows and dynamic pricing in the fashion industry.

---

## 📂 Project Context

The fashion industry is undergoing a digital transformation, where artificial intelligence plays a key role in both creative and business decision-making. Designers and retailers often require large volumes of visual content and struggle with pricing optimization due to subjectivity and seasonal demand patterns.

Generative models like DCGANs can automate image generation based on learned distributions of existing designs, while predictive models can estimate product prices based on image features and metadata. This dual approach allows fashion brands to:

- Prototype new designs faster
- Visualize product lines
- Optimize pricing strategies using data-driven insights

---

## 🎯 Project Objectives

1. **Fashion Content Generation**
   - Train a DCGAN on a curated dataset of fashion images, in this case, men's sneakers
   - Generate high-quality, diverse, and visually appealing fashion item images
   - Evaluate the realistic images using SSIM and Gini

2. **Price Prediction Model**
   - Convert images to tensors
   - Train regression models (Linear, XGBoost, Neural Nets) to predict prices from tensors
   - Optimize model performance using metrics like RMSE and R²

3. **Integration**
   - Build a pipeline that connects image generation with pricing prediction
   - Allow for on-the-fly estimation of the optimal price for generated fashion items

---

## 🛠️ Resources Used
The project leveraged the following resources

- **Fashion Fataset**: 
  - Fashion Dataset from Kaggle and Data World

- **Technologies & Tools**:
  - Python
  - Pandas
  - TensorFlow/Keras
  - OpenCV & PIL (image preprocessing)
  - Scikit-learn
  - Matplotlib, Seaborn (data visualization)
  - Jupyter Notebooks
  - 

- **Models**:
  - DCGAN (for image generation)
  - Regression models for price prediction (Linear Regression, Decision Tree, Random Forest Regression, Gradient Boost Regression, Support Vector Regression, K-Neighbours Regression, Lasso Regression)

---

## ✅ Results & Conclusion

- **Generation**:
  - Successfully trained a DCGAN capable of producing realistic fashion item images with minimal artifacts.
  - Achieved reasonable diversity in outputs, with room for further refinement using conditional GANs.

- **Price Optimization**:
  - Price prediction models achieved an RMSE below industry-acceptable thresholds on the test set.
  - Image-based features proved to be significant predictors of fashion item price, validating the approach.

- **Integration**:
  - Developed a working prototype that can generate fashion items and suggest a price instantly, offering significant utility for design prototyping and e-commerce decision-making.

---

## 📈 Future Work

- Implement Conditional GANs (cGAN) to control image attributes like color, type, and texture
- Add text-based attribute generation (e.g., generate image from product description)
- Deploy as a web app for real-time generation and pricing
