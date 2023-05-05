---
title: "Out-Of-Distribution Aware Model"
header_menu_title: "OOD Aware Model"
navigation_menu_title: "OOD Aware Model"
weight: 4
header_menu: true
---

Over the past half-decade there have been significant improvements in out-of-distribution (OOD) aware object detectors. Starting off, early approaches use post-hoc methods for evaluating whether objects are in-distribution (ID) or OOD. Simply thresholding maximum softmax probability on a pre-trained model improves OOD performance [2]. Taking things a step further, taking the "energy" of the softmax (proportional to area under the curve) further increases performance [3]. Another advantage of the energy score method is that unlike many other competitive OOD detection methods, such as ODIN [4] and Mahalanobis [5], it does not require hyperparameter tuning. Recent advances in OOD aware detectors take place during training-time. As an example, VOS [6] introduces a self-supervised approach at keeping queues of recent ID objects introduced during training. These queues are used to synthesize virtual outliers (which can be thought of as OOD objects) to train both the underlying network along with a ID/OOD-specific classification head.

![Equations](images/equations.png)
![Softmax vs Energy](images/softmax_vs_energy.png)
