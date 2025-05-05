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

## 🧠 Model Architecture

The model consists of:

- **Transformer Blocks** for capturing long-range spatial dependencies across modalities
- **Residual CNN Blocks** for texture recovery
- **Attention Fusion** to integrate RGB, QB, and TIR
- **Discriminator** for GAN training using a CNN classifier

Training involves:

- **Content Loss (L1)** + **Adversarial Loss**
- **PSNR/SSIM** used for evaluation
- **Mixed Precision Training** via PyTorch AMP

---

## 📸 Sample Outputs

Each result image below shows, from left to right:
**Low-Res Input → Super-Resolved Output → Ground Truth → Transformer Attention Heatmap**

| Sample Results            |
| ------------------------- |
| ![](results/Result_1.jpg) |
| ![](results/Result_2.jpg) |
| ![](results/Result_3.jpg) |
| ![](results/Result_4.jpg) |
| ![](results/Result_5.jpg) |
| ![](results/Result_6.jpg) |

---

## 🛠️ Tech Stack

- Python, PyTorch
- OpenCV, Matplotlib
- `torchmetrics`, `skimage.metrics`, `einops`
- Mixed Precision Training (AMP)

---

## 🧪 Applications

- 🌆 Urban Planning
- 🌍 Land Use Monitoring
- 🌿 Environmental Analysis
- 🛰️ Disaster Response

---

## 📚 Reference

This work was presented at:

**Applied Intelligence, Second International Conference (ICAI 2024)**  
📍 Zhengzhou, China — 🗓️ November 22–25, 2024  
📝 Proceedings, **Part II**, pp. **61–72**

---

## 📜 License

This repository is part of an academic submission. Please contact us for reuse or extension.

---

> Feel free to fork, star ⭐, or raise issues!
