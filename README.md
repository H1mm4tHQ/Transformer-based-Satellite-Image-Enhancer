# 🛰️ Transformer-Based Super-Resolution for Satellite Imagery

This project proposes a novel **Transformer-based Super-Resolution (SR)** model that enhances low-resolution satellite images using **geological context**. It integrates auxiliary modalities such as **QuickBird Panchromatic (QB)** and **Thermal Infrared (TIR)** images to improve spatial fidelity.

> ✨ Made by [Himmat](https://github.com/H1mm4tHQ) and [Anoop](https://github.com/anoopElGato) as part of a research-driven academic project.

---

## 🚀 Highlights

- 🧠 **Cross-Modality Attention**: RGB images query QB & TIR features to guide refinement.
- 🌀 **Hybrid Architecture**: Combines **transformers** for global context and **CNNs** for local texture enhancement.
- 🎯 **Adversarial Training**: Employs a **Transformer-GAN**, with a transformer-based generator and CNN-based discriminator.
- 📊 **Performance**:
  - PSNR: **33.87**
  - SSIM: **0.95**

---

## 📂 Dataset

- Sourced from [USGS Earth Explorer](https://earthexplorer.usgs.gov)
- Selected regions from **Northern India**
- Includes RGB, Panchromatic, and TIR imagery

---

## 🧪 Applications

- 🌆 Urban Planning
- 🌍 Land Use Monitoring
- 🌿 Environmental Analysis

---

## 📸 Sample Outputs

Each result image below shows, from left to right:
**Low-Res Input → Super-Resolved Output → Ground Truth → Transformer Attention Heatmap**

| Sample Results    |
| ----------------- |
| ![](result_1.jpg) |
| ![](result_2.jpg) |
| ![](result_3.jpg) |
| ![](result_4.jpg) |
| ![](result_5.jpg) |
| ![](result_6.jpg) |

---

## 🛠️ Tech Stack

- `PyTorch`, `OpenCV`, `Matplotlib`
- Transformer encoders + convolutional residual blocks
- GAN loss + content loss

---

## 🤝 Contributions

- `Himmat (H1mm4tHQ)`: Transformer integration, training pipeline, report
- `Anoop`: Data preprocessing, GAN design, evaluation

---

## 📜 License

This repository is part of an academic submission. Please contact us for reuse or extension.

---

> Feel free to fork, star ⭐, or raise issues!
