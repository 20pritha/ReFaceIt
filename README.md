# ReFaceIt - Sketch to 2D Face Reconstruction

ReFaceIt is a deep learning project that converts hand-drawn facial sketches into realistic facial photos using Generative Adversarial Networks (GANs). Designed to assist in law enforcement and forensic applications, the model reconstructs faces to aid in suspect identification and investigations where no real photos are available.
---

## 🧠 Problem Statement

Facial sketches are often the only visual reference in criminal investigations when photographs are unavailable. Our goal is to transform these sketches into realistic face images using AI, thereby improving recognition accuracy and aiding law enforcement.

---

## 💼 Business Use Cases

* Convert eyewitness sketches into photorealistic faces for suspect identification.
* Recreate faces of missing persons from sketches when photos are unavailable.
* Aid forensic reconstruction from skeletal remains or partial descriptions.

---

## 📊 Dataset Overview

### CUHK Face Sketch Dataset

* Contains paired hand-drawn sketches and real images.
* Sourced from datasets like CelebA.
* Requires preprocessing (resizing, normalization).
* Limitations: small dataset size, lack of annotations, less stylistic diversity.

---

## 📈 Exploratory Data Analysis (EDA)

* Resized images to 128x128 pixels.
* Normalized tensors and matched filenames.
* Rebalanced training/testing split for better performance.

---

## 🛠️ Methodology

### 1. GAN Architecture

* **Generator**: Converts sketches to realistic images.
* **Discriminator**: Distinguishes between real and generated images.
* **Training Loss**: Least Squares GAN (LSGAN) for stable learning.

### 2. Training Details

* **Optimizer**: Adam (LR=2e-4, β=(0.5, 0.999))
* **Epochs**: 100
* **Training Strategy**: Alternate updates for generator and discriminator
* **Visualization**: Output images displayed side-by-side using Matplotlib

---

## 📊 Results

* Trained model shows promising transformation from sketch to realistic image.
* Tracked training loss and SSIM (Structural Similarity Index) over epochs.

---

## 🚧 Challenges

* **Sketch Variability**: Styles differ drastically across artists.
* **Data Scarcity**: Limited high-quality paired datasets.
* **Hardware**: High-performance GPUs are essential for effective training.

---

## 🔗 References

* [Face Sketch to Image using GAN (GitHub)](https://github.com/Malikanhar/Face-Sketch-to-Image-Generation-using-GAN)
* [Face Sketch Recognition - ResearchGate Overview](https://www.researchgate.net/publication/341631538_Face_Sketch_Recognition-An_Overview)

---
