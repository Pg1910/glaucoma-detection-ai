# here all the basic informatics are shown about this project.
### model stacking flowchart showcasing our proposed pipeline
<img width="1889" height="791" alt="Screenshot 2025-07-07 191739" src="https://github.com/user-attachments/assets/9c888c49-d11c-4107-af53-57871c4383ca" />

# GlaucFusion: Segmentation-Aware Glaucoma Detection

**GlaucFusion** is a dual-branch Vision Transformer framework designed for robust and generalizable glaucoma detection. By combining segmentation-aware and global image-based representations, it achieves high accuracy across multiple benchmark datasets.

---

## Features

- **Dual-Branch Architecture**:
  - **Encoder-Only Mask Transformer (EOMT)**: Leverages optic disc/cup segmentation masks alongside fundus images.
  - **Domain-Adaptive DINOv2-ViT-S/14**: Dataset-specific classifiers for robust cross-domain performance.
- **Quality Control**: Laplacian variance filter automatically discards low-quality inputs.
- **Domain Mapping**: Dataset classification module routes inputs to the correct source domain.
- **Dynamic Fusion**: Confidence-weighted fusion module combines predictions from both branches based on their proximity to the decision boundary.

---

By fusing complementary features, GlaucFusion offers improved generalizability, interpretability, and reliability for automated glaucoma detection.
