# Awesome Incremental Object Detection

A single-page curated list for Incremental Object Detection (IOD), continual object detection, and related open-world object detection papers.

## Incremental Object Detection (IOD)

### Faster R-CNN

| Title | Venue / Year | Base detector / model | Main idea |
| --- | --- | --- | --- |
| [Modeling Missing Annotations for Incremental Learning in Object Detection](https://openaccess.thecvf.com/content/CVPR2022W/CLVision/papers/Cermelli_Modeling_Missing_Annotations_for_Incremental_Learning_in_Object_Detection_CVPRW_2022_paper.pdf) | CVPRW 2022 | Faster R-CNN | Models missing annotations in RPN/RCN to reduce wrong background supervision for old/future classes. |
| [Bridge Past and Future: Overcoming Information Asymmetry in Incremental Object Detection](https://arxiv.org/abs/2407.11499) | ECCV 2024 | Faster R-CNN | Bridges old, current, and future class information using old-class pseudo labels, future-object suppression, and Distillation with Future. |
| [Gradient Decomposition and Alignment for Incremental Object Detection](https://openaccess.thecvf.com/content/ICCV2025/papers/Luo_Gradient_Decomposition_and_Alignment_for_Incremental_Object_Detection_ICCV_2025_paper.pdf) | ICCV 2025 | Faster R-CNN + ResNet-50 | Uses GMM pseudo labels and gradient decomposition/alignment to balance old-class stability and new-class plasticity. |
| [Demystifying Catastrophic Forgetting in Two-Stage Incremental Object Detector](https://icml.cc/virtual/2025/poster/45396) | ICML 2025 | Faster R-CNN | Identifies RoI head classifier forgetting and proposes Regional Prototype Replay with Null Space Gradient Projection. |
| [High-dimension Prototype is a Better Incremental Object Detection Learner](https://openreview.net/forum?id=6T8czSBWce) | ICLR 2025 | ILOD / ABR style KD-based IOD | Uses Gaussian Mixture Distribution-based high-dimensional prototypes to reduce knowledge shift. |
| [Interference-Isolated Elastic Weight Consolidation and Knowledge Calibration for Incremental Object Detection](https://openreview.net/pdf?id=VrXdmCjni4) | ICLR 2026 | Faster R-CNN | Uses interference-isolated EWC and prototype knowledge calibration to preserve old-class discriminability. |

### ViTDet / Mask R-CNN

| Title | Venue / Year | Base detector / model | Main idea |
| --- | --- | --- | --- |
| [Learning Endogenous Attention for Incremental Object Detection](https://openaccess.thecvf.com/content/CVPR2025/papers/Song_Learning_Endogenous_Attention_for_Incremental_Object_Detection_CVPR_2025_paper.pdf) | CVPR 2025 | ViTDet; ViT backbone + Mask R-CNN head | Converts image-to-annotation alignment into annotation-to-instance alignment with task-specific endogenous attention modules and an energy-based task modulator. |

### DETR

| Title | Venue / Year | Base detector / model | Main idea |
| --- | --- | --- | --- |
| [Preventing Catastrophic Forgetting through Memory Networks in Continuous Detection](https://arxiv.org/pdf/2403.14797) | ECCV 2024 | Pretrained DETR-style detector + memory network | Adds memory units and localized queries, and addresses background relegation in continual detection. |
| [DCA: Dividing and Conquering Amnesia in Incremental Object Detection](https://arxiv.org/pdf/2503.15295) | AAAI 2025 | Deformable DETR / D-DETR | Separates localization and recognition, then uses PLM semantic queries to strengthen old-class recognition. |
| [PseDet: Revisiting the Power of Pseudo Label in Incremental Object Detection](https://openreview.net/pdf?id=Iu8FVcUmVp) | ICLR 2025 | GFL; Deformable DETR | Improves pseudo-label quality through spatio-temporal enhancement, adaptive class thresholds, and score calibration. |
| [Better Matching, Less Forgetting: A Quality-Guided Matcher for Transformer-based Incremental Object Detection](https://arxiv.org/pdf/2603.01524) | AAAI 2026 | Deformable DETR; DN-DETR / DAB-DETR validation | Replaces forced Hungarian assignment with Q-MCMF to avoid low-quality supervision and background foregrounding. |

### Pretrained / Vision-Language Models

| Title | Venue / Year | Base detector / model | Main idea |
| --- | --- | --- | --- |
| [Learning Task-Aware Language-Image Representation for Class-Incremental Object Detection](https://csgaobb.github.io/Pub_files/AAAI2024_CIOD.pdf) | AAAI 2024 | GLIP-style language-image detector | Learns task-aware language-image representations and uses task-specific alignment scores for selective inference. |
| [GCD: Advancing Vision-Language Models for Incremental Object Detection via Global Alignment and Correspondence Distillation](https://ojs.aaai.org/index.php/AAAI/article/view/32864) | AAAI 2025 | Grounding-DINO-T | Uses global semantic alignment and semantic correspondence distillation to preserve text-vision structures. |
| [YOLO-IOD: Towards Real Time Incremental Object Detection](https://arxiv.org/pdf/2512.22973) | AAAI 2026 | Pretrained YOLO-World | Builds a real-time IOD framework with pseudo-label refinement, important-kernel selection, and cross-stage asymmetric distillation. |

## Open-World Object Detection

### Objectness Perspective

| Title | Venue / Year | Main idea |
| --- | --- | --- |
| [OW-DETR: Open-World Detection Transformer](https://openaccess.thecvf.com/content/CVPR2022/html/Gupta_OW-DETR_Open-World_Detection_Transformer_CVPR_2022_paper.html) | CVPR 2022 | Adds explicit objectness scoring to DETR with attention-driven pseudo-labeling and novelty classification to separate unknown objects from background. |
| [PROB: Probabilistic Objectness for Open World Object Detection](https://openaccess.thecvf.com/content/CVPR2023/html/Zohar_PROB_Probabilistic_Objectness_for_Open_World_Object_Detection_CVPR_2023_paper.html) | CVPR 2023 | Models objectness as probability density / likelihood in embedding space to improve unknown-object recall without requiring unknown-class negative supervision. |
| [Open-World Objectness Modeling Unifies Novel Object Detection](https://openaccess.thecvf.com/content/CVPR2025/papers/Zhang_Open-World_Objectness_Modeling_Unifies_Novel_Object_Detection_CVPR_2025_paper.pdf) | CVPR 2025 | Jointly models generic objectness and class labels with a dynamic Gaussian prior and energy-based margin loss for novel-object discovery. |
