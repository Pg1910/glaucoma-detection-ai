# here all the basic informatics are shown about this project.
### model stacking flowchart showcasing our proposed pipeline
<img width="1889" height="791" alt="Screenshot 2025-07-07 191739" src="https://github.com/user-attachments/assets/9c888c49-d11c-4107-af53-57871c4383ca" />

GlaucFusion
Glaucoma is a leading cause of irreversible blindness, often progressing silently until advanced stages. Early and accurate detection is critical for preventing vision loss.

GlaucFusion is a dual-branch Vision Transformer framework designed for robust and generalizable glaucoma diagnosis. Our approach integrates segmentation-aware and global image-based representations for improved accuracy across diverse datasets.

Key Features

Dual-Branch Architecture:

Encoder-Only Mask Transformer (EOMT): Leverages optic disc/cup segmentation masks along with fundus images.

Domain-Adaptive DINOv2-ViT-S/14: Uses dataset-specific classifiers to adapt to different sources.

Quality Control: Laplacian variance filter automatically discards low-quality inputs.

Domain Mapping: Dataset classification module routes inputs to the correct domain.

Dynamic Fusion: Confidence-weighted fusion module combines predictions from both branches based on their proximity to the decision boundary.

Conclusion

By fusing complementary features, GlaucFusion offers improved generalizability, interpretability, and reliability for automated glaucoma detection.
