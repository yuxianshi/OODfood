---
title: "Challenge"
weight: 3
header_menu: true
---

The training of the food image classification model requires labeled images. Though the food captions and reviews can be helpful in creating such labels, they may be imprecise and are often limited in amount. Therefore, to ensure a large amount of reliably labeled data, we do not restrict to images of one restaurant when training the classification model which will be used on this restaurant. Instead, we turn to publicly available data sets with relatively reliable labels and large size. The training data that we have preliminarily chosen for this project is the food-101 data [1], which contains 101,000 labeled food images in 101 categories collected from foodspotting.com (acquired by OpenTable in 2013). With the convenience of obtaining a large training data set comes the challenge of out-of-distribution prediction, since the images on which the model will be applied may differ in various aspects from those in the training data, as they are collected from different restaurants and different websites. In particular, while the food-101 data contains only food images, in real-world application scenarios, food images are often mixed with non-food images of, e.g., restaurant inside/outsie, menus, receipts, etc. To address this challenge, this project will focus on out-of-distribution (OOD) aware image classification methods.

In addition, at test time, we are interested in evaluating OOD detection in the real-world scenario of mapping menu items to food images, in spite of that most proposed OOD detection methods have only been tested on standard benchmarks. More specificlly, We will test our OOD detection methods using images aquired from Yelp.com. We hope that this will give us a more realistic impression of the utility of OOD detection in the food domain.

![OOD](images/ood.png)