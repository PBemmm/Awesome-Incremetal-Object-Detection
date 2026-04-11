# Awesome Open-World Object Detection

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated collection of papers, codebases, benchmarks, datasets, and survey resources for **Open-World Object Detection (OWOD)**, together with closely related **Incremental Object Detection (IOD)**, **Class-Incremental Object Detection (CIOD)**, and other continual detection settings.

This repository aims to be a clean, long-term maintained entry point for researchers and practitioners who want to quickly understand the landscape of open-world and incremental object detection: task settings, representative methods, evaluation protocols, and public implementations.

## Recommended Repository Name

The repository is now positioned as:

`awesome-open-world-object-detection`

Short alias:

`awesome-OWOD`

Why this name works well:

- Clear and unambiguous for new visitors
- Search-friendly on GitHub and Google
- Clear OWOD-first positioning for the repository brand
- Still flexible enough to include related IOD and CIOD resources
- Strong keyword match for a recognizable subfield

## Scope

This repository mainly tracks:

- Open-world object detection papers
- Incremental / continual object detection papers closely related to OWOD
- Survey and perspective papers
- Public codebases and project pages
- Benchmarks, datasets, and evaluation protocols
- Training recipes, settings, and comparison resources

Out of scope by default:

- Generic continual learning papers without a detection component
- Pure open-vocabulary detection unless there is a clear OWOD or continual detection setting
- Incremental segmentation papers unless they directly include object detection

## Current Collection

- Surveys: [lists/surveys.md](lists/surveys.md)
- Core papers: [lists/papers.md](lists/papers.md)
- Benchmarks and datasets: [lists/benchmarks.md](lists/benchmarks.md)
- Codebases and toolkits: [lists/codebases.md](lists/codebases.md)

## Starter Reading List

If you are new to the area, a practical reading order is:

1. [Towards Open World Object Detection (CVPR 2021)](https://openaccess.thecvf.com/content/CVPR2021/html/Joseph_Towards_Open_World_Object_Detection_CVPR_2021_paper.html)
2. [OW-DETR: Open-World Detection Transformer (CVPR 2022)](https://openaccess.thecvf.com/content/CVPR2022/html/Gupta_OW-DETR_Open-World_Detection_Transformer_CVPR_2022_paper.html)
3. [PROB: Probabilistic Objectness for Open World Object Detection (CVPR 2023)](https://openaccess.thecvf.com/content/CVPR2023/html/Zohar_PROB_Probabilistic_Objectness_for_Open_World_Object_Detection_CVPR_2023_paper.html)
4. [Random Boxes Are Open-world Object Detectors (ICCV 2023)](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Random_Boxes_Are_Open-world_Object_Detectors_ICCV_2023_paper.html)
5. [Exploring Orthogonality in Open World Object Detection (CVPR 2024)](https://openaccess.thecvf.com/content/CVPR2024/html/Sun_Exploring_Orthogonality_in_Open_World_Object_Detection_CVPR_2024_paper.html)
6. [Open World Object Detection: A Survey (arXiv / TCSVT)](https://arxiv.org/abs/2410.11301)

## Suggested Main Table Format

For long-term maintenance, use a single compact format for paper entries:

| Year | Venue | Paper | Setting | Method Tags | Protocol / Dataset | Code |
| --- | --- | --- | --- | --- | --- | --- |
| 2024 | CVPR | Paper Title | `CIOD` | `Replay`, `Distill`, `Transformer` | `COCO 40+40` | [Code](#) |

## Tag Taxonomy

To keep the list readable, use a small set of consistent tags instead of free-form notes.

### 1. Setting Tags

- `IOD`: Incremental Object Detection
- `CIOD`: Class-Incremental Object Detection
- `OWOD`: Open-World Object Detection
- `CDOD`: Continual Domain Object Detection
- `Survey`: Survey / review / perspective

### 2. Method Tags

- `Replay`: rehearsal, memory, exemplar replay
- `Distill`: knowledge distillation or teacher-student transfer
- `Regularize`: parameter or feature regularization
- `Expand`: dynamic architecture expansion or extra branches
- `Objectness`: class-agnostic objectness or unknownness modeling
- `Pseudo-label`: pseudo-unknown mining or automatic unknown labeling
- `Probabilistic`: uncertainty, density, or probabilistic foreground modeling
- `Prompt`: prompt-based or query-guided adaptation
- `Prototype`: prototype, class-center, or cluster-based methods
- `Generate`: synthetic replay or generative modeling
- `Adapter`: adapter, LoRA, or lightweight parameter tuning
- `Meta`: meta-learning or optimization-based adaptation

### 3. Detector Tags

- `Two-stage`
- `One-stage`
- `Transformer`

### 4. Resource Tags

- `Code`
- `Benchmark`
- `Dataset`

## Repository Structure

```text
awesome-open-world-object-detection/
|- README.md
|- assets/
|  `- README.md
|- docs/
|  |- taxonomy.md
|  `- paper-template.md
`- lists/
   |- surveys.md
   |- papers.md
   |- benchmarks.md
   `- codebases.md
```

## List Organization

Recommended top-level sections:

1. Surveys
2. Core Papers
3. Benchmarks and Datasets
4. Codebases and Toolkits
5. Evaluation Protocols and Settings

If the repo grows larger, split the paper list into:

- `CIOD`
- `OWOD`
- `CDOD`
- `Related Continual Detection`

## Contribution Workflow

To keep this repo maintainable:

- Use the tag system defined in [docs/taxonomy.md](docs/taxonomy.md)
- Add new entries with the template in [docs/paper-template.md](docs/paper-template.md)
- Prefer official paper links, official code links, and canonical project pages
- Keep notes short and factual
- Avoid duplicate entries across sections

## Starter Plan

A practical first milestone for this repository:

1. Add 1 to 3 survey papers
2. Add representative CIOD papers
3. Add representative OWOD papers
4. Add benchmark protocols such as VOC / COCO splits
5. Add official code repositories for the most cited methods

## License

This repository is intended as a community-curated resource list. Please respect the licenses of linked papers, codebases, datasets, and external assets.
