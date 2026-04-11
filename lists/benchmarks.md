# Benchmarks and Datasets

Recommended columns:

| Name | Type | Setting | Description | Link |
| --- | --- | --- | --- | --- |
| PASCAL VOC OWOD protocol | Protocol | `OWOD` | Canonical staged open-world benchmark used from ORE onward for unknown discovery and incremental class expansion | [ORE paper](https://openaccess.thecvf.com/content/CVPR2021/html/Joseph_Towards_Open_World_Object_Detection_CVPR_2021_paper.html) |
| MS-COCO OWOD protocol | Protocol | `OWOD` | Large-scale OWOD benchmark widely reported by OW-DETR, PROB, CAT, and RandBox | [OW-DETR paper](https://openaccess.thecvf.com/content/CVPR2022/html/Gupta_OW-DETR_Open-World_Detection_Transformer_CVPR_2022_paper.html) |
| PASCAL VOC incremental splits (`19+1`, `15+5`, `10+10`) | Protocol | `IOD` | Standard class-incremental detection settings used by early and recent IOD papers | [ICCV 2017 paper](https://openaccess.thecvf.com/content_iccv_2017/html/Shmelkov_Incremental_Learning_of_ICCV_2017_paper.html) |
| MS-COCO incremental split (`40+40`) | Protocol | `IOD` | Common large-scale incremental detection protocol reported by iOD and follow-up work | [iOD codebase](https://github.com/JosephKJ/iOD) |
| M-OWODB | Benchmark | `OWOD` | Superclass-mixed OWOD benchmark used by newer methods to stress class overlap and open-world transfer | [OrthogonalDet](https://github.com/feifeiobama/OrthogonalDet) |
| S-OWODB | Benchmark | `OWOD` | Superclass-separated OWOD benchmark used alongside M-OWODB for more fine-grained staged evaluation | [OrthogonalDet](https://github.com/feifeiobama/OrthogonalDet) |
