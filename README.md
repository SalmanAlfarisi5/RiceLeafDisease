# Rice-Leaf Disease Classification 🌾

A compact pipeline for detecting rice-leaf diseases using deep-learning models trained on a five-class image dataset.

---

## 📦 Dataset

| Item                     | Detail                               |
|--------------------------|--------------------------------------|
| Source                   | Rice leaf disease detection dataset  |
| Classes                  | **5** – `Healthy`, plus **4** disease types |
| Image resolution         | `224 × 224 × 3` (RGB)                |

---

## 🎯 Project Objectives

* **Balanced split** – every 5th image (per class) → **test set** (≈ 20 %), remainder → **train** (≈ 80 %).
* **Transfer-learning experiments** – compare multiple pretrained CNN backbones.
* **Custom CNN** – evaluate a small network trained from scratch.
* **Error analysis** – list and inspect every mis-classified sample to guide data cleaning / augmentation.

---

## 🧪 Experiments & Results

| Model              | Best Train Acc | Best Test Acc |
|--------------------|:--------------:|:-------------:|
| MobileNet V2       | **1.0000**     | **0.9882** |
| EfficientNet B0    | **1.0000**     | **0.9941** |
| ResNet-50          | **1.0000**     | **1.0000** |
| Custom CNN (scratch)| 0.8671        | 0.8824 |

*All scores are top-1 accuracies after fine-tuning with early stopping.*

---
