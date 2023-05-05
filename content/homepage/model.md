---
title: "Model Training"
header_menu_title: "Model Training"
navigation_menu_title: "Model Training"
weight: 5
header_menu: true
---

Our approach to creating reliable food classifiers consisted of two parts. First, we trained a ResNet architecture classifier [7] on the Food-101 dataset (75%). Previously unused images from the Food-101 dataset (25%) were then added to a new evaluation set, which was supplemented with OOD images from Yelp.com (91948 images in total). These OOD images are selected from the Yelp data set using the provided image meta data; we included all images having a non-food label. We ran this evaluation set against our "vanilla" trained model alongside a model using the energy-score post-hoc method [3] for more robust classification. Overall, our approach involved re-implementing prior solutions on new domains.
