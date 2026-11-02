# Understand Before Detect: Vision–Language Learning for Omni-Domain Infrared Small Target Detection

[![arXiv](https://img.shields.io/badge/arXiv-2608.07015-b31b1b.svg)](https://arxiv.org/abs/2608.07015)

**Official repository for [*Understand Before Detect: Vision–Language Learning for Omni-Domain Infrared Small Target Detection*](https://arxiv.org/abs/2608.07015).**

This repository will host **JinSight**, our vision–language framework for omni-domain infrared small target detection, and **OmniIRST-VL**, our infrared vision–language dataset.

## Overview

Conventional infrared small target detection methods primarily rely on binary target–background supervision, which overlooks rich scene semantics and target–context relationships. We introduce an **“understand before detect”** paradigm that learns holistic infrared understanding before transferring the learned representations to precise small target detection.

- **JinSight:** A two-stage framework that first performs IRST-oriented visual instruction tuning and then adapts the learned representations for detection and segmentation.
- **OmniIRST-VL:** A dataset with **39,701 image–instruction–response pairs** built from **11,000 infrared images**, spanning diverse platforms, spectral bands, and scene conditions. It covers detailed captioning (9228), physical VQA (9000), and image-/region-level counting (13,713) and grounding (7,760).

On WideIRSTD, JinSight achieves **73.75% detection probability (Pd)** and **42.94% IoU**. See the [paper](https://arxiv.org/abs/2608.07015) for experimental details.

## Release Roadmap

We plan to release the dataset and original implementation in stages. The following checklist will be updated as resources become available.

### Dataset

- [ ] Release **OmniIRST-VL** annotations and instruction–response pairs.
- [ ] Release dataset splits, task definitions, and data preparation instructions.
- [ ] Release the **OmniIRST-Benchmark** and evaluation protocol.

### Source Code

- [ ] Release the original **JinSight** implementation.
- [ ] Release Stage I visual instruction tuning code.
- [ ] Release Stage II detection/segmentation code, including **LSI**.
- [ ] Release training configurations, evaluation scripts, and reproduction instructions.

### Model Weights

- [ ] Release pretrained **JinSight-1B** weights.

## Citation

If you find this work useful, please consider citing our paper:

```bibtex
@misc{yuan2026understand,
  title = {Understand Before Detect: Vision--Language Learning for Omni-Domain Infrared Small Target Detection},
  author = {Haoyang Yuan and Boyang Li and Yingqian Wang and Yimian Dai and Nuo Chen and Xinfei Huang and Shuqi Yi and Zaiping Lin and Weidong Sheng and Wei An},
  year = {2026},
  eprint = {2608.07015},
  archivePrefix = {arXiv},
  primaryClass = {cs.CV},
  url = {https://arxiv.org/abs/2608.07015}
}
```

## Contact

For questions or updates, please open an [issue](https://github.com/shushengyuan/OmniIRSTD-VL/issues) in this repository.
