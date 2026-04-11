# Core Papers

This list is intended for OWOD papers first, with closely related IOD / CIOD papers included when they help readers understand the broader landscape.

Recommended columns:

| Year | Venue | Paper | Setting | Method Tags | Protocol / Dataset | Code |
| --- | --- | --- | --- | --- | --- | --- |
| 2021 | CVPR | [Towards Open World Object Detection](https://openaccess.thecvf.com/content/CVPR2021/html/Joseph_Towards_Open_World_Object_Detection_CVPR_2021_paper.html) | `OWOD` | `Objectness`, `Pseudo-label`, `Two-stage` | `VOC / COCO OWOD` | [Code](https://github.com/JosephKJ/OWOD) |
| 2022 | CVPR | [OW-DETR: Open-World Detection Transformer](https://openaccess.thecvf.com/content/CVPR2022/html/Gupta_OW-DETR_Open-World_Detection_Transformer_CVPR_2022_paper.html) | `OWOD` | `Transformer`, `Objectness`, `Pseudo-label` | `VOC / COCO OWOD` | [Code](https://github.com/akshitac8/OW-DETR) |
| 2023 | CVPR | [PROB: Probabilistic Objectness for Open World Object Detection](https://openaccess.thecvf.com/content/CVPR2023/html/Zohar_PROB_Probabilistic_Objectness_for_Open_World_Object_Detection_CVPR_2023_paper.html) | `OWOD` | `Transformer`, `Objectness`, `Probabilistic` | `VOC / COCO OWOD` | [Code](https://github.com/orrzohar/PROB) |
| 2023 | CVPR | [CAT: LoCalization and IdentificAtion Cascade Detection Transformer for Open-World Object Detection](https://openaccess.thecvf.com/content/CVPR2023/html/Ma_CAT_LoCalization_and_IdentificAtion_Cascade_Detection_Transformer_for_Open-World_Object_CVPR_2023_paper.html) | `OWOD` | `Transformer`, `Pseudo-label`, `Objectness` | `VOC / COCO OWOD` | `-` |
| 2023 | ICCV | [Random Boxes Are Open-world Object Detectors](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Random_Boxes_Are_Open-world_Object_Detectors_ICCV_2023_paper.html) | `OWOD` | `Objectness`, `Regularize`, `Two-stage` | `VOC / COCO OWOD`, `LVIS` | [Code](https://github.com/scuwyh2000/RandBox) |
| 2024 | CVPR | [Exploring Orthogonality in Open World Object Detection](https://openaccess.thecvf.com/content/CVPR2024/html/Sun_Exploring_Orthogonality_in_Open_World_Object_Detection_CVPR_2024_paper.html) | `OWOD` | `Regularize`, `Objectness`, `Two-stage` | `M-OWODB / S-OWODB` | [Code](https://github.com/feifeiobama/OrthogonalDet) |

## Related IOD / CIOD Papers

| Year | Venue | Paper | Setting | Method Tags | Protocol / Dataset | Code |
| --- | --- | --- | --- | --- | --- | --- |
| 2017 | ICCV | [Incremental Learning of Object Detectors Without Catastrophic Forgetting](https://openaccess.thecvf.com/content_iccv_2017/html/Shmelkov_Incremental_Learning_of_ICCV_2017_paper.html) | `IOD` | `Distill`, `Two-stage` | `VOC 19+1`, `COCO incremental` | `-` |
| 2021 | TPAMI | [Incremental Object Detection via Meta-Learning](https://arxiv.org/abs/2003.08798) | `IOD` | `Meta`, `Distill`, `Two-stage` | `VOC 19+1`, `15+5`, `10+10`; `COCO 40+40` | [Code](https://github.com/JosephKJ/iOD) |
| 2022 | CVPRW | [Modeling Missing Annotations for Incremental Learning in Object Detection](https://openaccess.thecvf.com/content/CVPR2022W/CLVision/html/Cermelli_Modeling_Missing_Annotations_for_Incremental_Learning_in_Object_Detection_CVPRW_2022_paper.html) | `CIOD` | `Distill`, `Regularize`, `Two-stage` | `VOC 19+1`, `15+5`, `10+10`, multi-step | [Code](https://github.com/fcdl94/MMA) |
