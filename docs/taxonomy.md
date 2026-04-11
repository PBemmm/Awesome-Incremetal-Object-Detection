# Taxonomy and Tagging Rules

This document defines a small and stable tag system for maintaining an **OWOD-first** repository that also includes closely related IOD / CIOD directions.

## Design Principles

- Keep tags short and reusable
- Prefer controlled vocabulary over free-form descriptions
- Separate the task setting from the method family
- Use at most 3 to 5 tags per paper row

## Required Fields for Each Paper Entry

Each paper entry should include:

- `Year`
- `Venue`
- `Paper`
- `Setting`
- `Method Tags`
- `Protocol / Dataset`
- `Code`

## Setting Tags

- `IOD`: generic incremental object detection when the paper does not fit a narrower label
- `CIOD`: new classes are introduced over stages while retaining old-class detection ability
- `OWOD`: unknown objects and known-class expansion are both part of the setting
- `CDOD`: the domain changes across stages while detection is continually adapted
- `Survey`: surveys, reviews, perspectives, or benchmark summaries

## Method Tags

- `Replay`: exemplar storage, feature replay, or memory rehearsal
- `Distill`: response, logit, feature, relation, or localization distillation
- `Regularize`: anti-forgetting constraints, parameter penalties, or stability losses
- `Expand`: dynamic heads, branches, modules, or parameter growth
- `Objectness`: class-agnostic objectness or unknown-vs-background modeling
- `Pseudo-label`: pseudo-unknown mining, automatic relabeling, or proposal relabeling
- `Probabilistic`: uncertainty, density estimation, or probabilistic objectness modeling
- `Prompt`: prompt learning, query tuning, or instruction-conditioned adaptation
- `Prototype`: prototype banks, class centers, or metric learning based retention
- `Generate`: generative replay, pseudo-instance synthesis, or data generation
- `Adapter`: adapters, LoRA-style updates, or parameter-efficient continual tuning
- `Meta`: meta-learning or optimization-based task adaptation

## Detector Tags

- `Two-stage`: Faster R-CNN style methods
- `One-stage`: YOLO, RetinaNet, FCOS style methods
- `Transformer`: DETR and query-based detector families

## Resource Tags

- `Code`: official or reliable public implementation exists
- `Benchmark`: benchmark suite or protocol contribution
- `Dataset`: dataset or split release

## Recommended Row Style

```md
| 2024 | CVPR | [Paper Title](paper-link) | `CIOD` | `Replay`, `Distill`, `Transformer` | `COCO 40+40` | [Code](code-link) |
```

## Tagging Tips

- If a paper belongs to OWOD, prefer `OWOD` over the more generic `IOD`
- If the method uses multiple ideas, choose the dominant 2 to 3 method tags only
- Use detector tags only when they add comparison value
- Do not invent new tags unless several papers clearly need the same concept
