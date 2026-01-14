---
layout: page
title: Food identification.
description: Creating a dataset for food identification and training a YOLO model.
img: assets/img/research/vegi_nutrition.jpg
importance: 3
category: Vision
related_publications: false
---

## Overview

This research area combines computer vision, deep learning, and practical applications to solve a critical problem of food type wich containts iron for edutational in anemia context . My work focuses on create a dataset for food identification and training a proper model to detect food items and estimate the iron content, we did a deep exploration about what is the anemia and nutrition mean and how to select the foods available in the south peruvian context, we also did a deep exploration about the YOLO model and how to fine-tune it for our specific use case. and finally make this available in a paper(under review)

---
### Vegetable and Fruit Detection Using YOLO

In this project, I fine-tuned the YOLO (You Only Look Once) algorithm to detect various vegetables and fruits using a local dataset. By leveraging transfer learning techniques, I improved detection accuracy and performance for real-time applications. The model demonstrates robust capabilities in distinguishing between different produce items, making it suitable for applications in agriculture, retail, and smart kitchen.

<div class="row  justify-content-sm-center ">
    <div class="col-sm mt-3 mt-md-0">
        <a href="{{ site.baseurl }}/assets/img/projects/19.jpg" data-fancybox="project" title="Example Image" class="zoom" >
        {% include figure.liquid path="assets/img/projects/19.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
        </a>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/gRzWhL-86Gg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    the image preview of the set of images trained as batch in the left, and test step for the fine-tuned model video(in the right).
</div>

---
{% comment %}
### images segmentation using SAM

<div class="row  justify-content-sm-center ">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/16.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/mZdsx-WhCwo" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


{% endcomment %}

---

*For collaboration opportunities or to discuss potential projects, please [contact me](/contact/).*
