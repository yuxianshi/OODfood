---
title: "Results"
weight: 6
header_menu: true
---

Our evaluation set was a mix of the Food-101 dataset alongside an open-source Yelp dataset. The Food-101 dataset served for ID evaluation and the Yelp dataset served to characterize the real-world/OOD performance of the model. For metrics, we focused on the false positive rate (FPR) and mean average precision (MAP). 


**Base model** 

* 71% accuracy after 250 epochs of training
* 82% accuracy after 250 epochs of training (pretrained)

**After including OOD**

| FPR95 | AUROC | AUPR | mAP |
| --- | --- | --- | --- |
| 54.13% | 90.07% | 97.94% | 82.1% |