---
title: "Food Image Classification & Motivation"
header_menu_title: "Problem & Motivation"
navigation_menu_title: "Problem & Motivation"
weight: 2
header_menu: true
---
![Food Classification](images/motivation.png)

Food plays an important role of everyday life and, as a common place for having food, restaurants not only deliver the enjoyment of food themselves, but also provide us a space for experiencing different cultures, through food from various cuisine styles. One frequent barrier for having food from a different culture, though, is that the menus can be hard to understand. This is often experienced by international travelers, as well as by people who live far away from where they grew up. One reason for this barrier is that dish names can be hard to translate and a sufficient description of a dish is usually too long to be put on a menu. While names and descriptions on menus may be hard to comprehend, photos are much more effective in conveying the idea of dishes.  With a glance, photos can tell whether a dish is soupy, rich in vegetable, heavily cooked or relatively fresh, and  small or large in portion size. Therefore, a potentially useful tool for aiding foreign customers is a mapping between menu items and its corresponding food images posted by customers of the restaurant. With a suitable API, this mapping may allow customers to view photos of a dish by just clicking a menu item.

![Menu Mapping](images/mapping.png)

In order to create the menu to photo mapping, one needs to label each food image with a menu item. While some images posted on food review/delivery websites are accompanied by a caption or review, many are not. Moreover, despite that the captions and reviews may be useful for labeling images, they are often loose descriptions and may include more than one dish. Thus, a classification method is required to process and label all images of a restaurant.


