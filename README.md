# AnoRefiner

**This is an official PyTorch implementation for "AnoRefiner: Anomaly-Aware Group-Wise Refinement for Zero-Shot Industrial Anomaly Detection"**

Authors: [Dayou Huang](https://github.com/d339293440)<sup>1</sup> | [Feng Xue](https://xuefeng-cvr.github.io/)<sup>3</sup> | [Xurui Li](https://github.com/xrli-U)<sup>1</sup> | [Yu Zhou](https://github.com/zhouyu-hust)<sup>1,2</sup>

Institutions: <sup>1</sup>Huazhong University of Science and Technology | <sup>2</sup>Wuhan JingCe Electronic Group Co.,LTD | <sup>3</sup>University of Trento

### 🧐 [Arxiv](https://arxiv.org/abs/2511.22595)

## TODO

Our paper is currently under review. We plan to make the complete code repository public upon its acceptance.

## 👇Abstract

Zero-shot industrial anomaly detection (ZSAD) methods typically yield coarse anomaly maps as vision transformers (ViTs) extract patch-level features only. To solve this, recent solutions attempt to predict finer anomalies using features from ZSAD, but they still struggle to recover fine-grained anomalies without missed detections, mainly due to the gap between randomly synthesized training anomalies and real ones. We observe that anomaly score maps exactly provide complementary spatial cues that are largely absent from ZSAD's image features, a fact overlooked before.

Inspired by this, we propose an anomaly-aware refiner (AnoRefiner) that can be plugged into most ZSAD models and improve patch-level anomaly maps to the pixel level.
First, we design an anomaly refinement decoder (ARD) that progressively enhances image features using anomaly score maps, reducing the reliance on synthetic anomaly data. Second, motivated by the mass production paradigm, we propose a progressive group-wise test-time training (PGT) strategy that trains ARD in each product group for the refinement process in the next group, while staying compatible with any ZSAD method.

Experiments on the MVTec AD and VisA datasets show that AnoRefiner boosts various ZSAD models by up to a 5.2\% gain in pixel-AP metrics, which can also be directly observed in many visualizations.

## Citation:
```
@inproceedings{arxiv2025AnoRefiner,
  title={AnoRefiner: Anomaly-Aware Group-Wise Refinement for Zero-Shot Industrial Anomaly Detection},
  author={Huang, Dayou and Xue, Feng and Li, Xurui and Zhou, Yu},
  journal={arXiv preprint arXiv:2511.22595},
  year={2025}
}
```

## License:
AnoRefiner is released under the **MIT Licence**, and is fully open for academic research and also allow free commercial usage. To apply for a commercial license, please contact yuzhou@hust.edu.cn.
