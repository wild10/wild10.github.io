---
layout: page
title: 3D reconstruction
description: 3D Image reconstruction using multiresolution hierarchies.
img: assets/img/projects/3d_image.png
importance: 4
category: Computer Vision
---

### 3D Image reconstruction

##### multiresolution hierarchies

Many tasks in geometry processing and physical simulation benefit from multiresolution hierarchies. In this project i aimed to re-implement and run this method to explore thi existing techniques such as surface mesh decimation, voxelization.The method constructs each next-coarsest level of the hierarchy using a sequence of decimation, flow. I also learnt using OPenGL,mesh with c++ and all the framework related to 3D analysis

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        <a href="{{ site.baseurl }}/assets/img/projects/11.jpg" data-fancybox="project" title="Example Image" class="zoom" >
            {% include figure.liquid path="assets/img/projects/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
        </a>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/qZCHblf1YMs" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The Images shows 3D reconstruction for bunny(nested cage method) and face reconstruction.
</div>

<ul>
    <li> Nested Cages: 
    :scroll: <a href="https://www.cs.columbia.edu/cg/nested-cages/nested-cages-siggraph-asia-2015-sacht-et-al.pdf"> paper </a>
    :rocket:  <a href="https://github.com/wild10/ImplementationReview_NestedCages"> git_repo </a>    
    :play_or_pause_button: <a href="https://www.youtube.com/watch?v=qZCHblf1YMs"> video_youtube_here </a>
    </li>
</ul>

--- 
##### 3D Face Reconstruction from a Single Image

3D face reconstruction is a fundamental Computer Vision problem of extraordinary difficulty. this paper uses a single image as input and i prove their effectiveness by running the code and using only one image(2D) that uses the CNN and facial landmark localization methods.

<div class="row  justify-content-sm-center ">
    <div class="col-sm mt-3 mt-md-0">
         <a href="{{ site.baseurl }}/assets/img/projects/3.png" data-fancybox="project" title="Example Image" class="zoom" >
            {% include figure.liquid path="assets/img/projects/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </a>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/XWRRvUBN1wk" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    The image in the left shows, the paper output and method and the videos in the right presents my own re-implementation for Action recognition Dataset.
</div>

<ul>
    <li>  3D Face Reconstruction from a Single Image ,Direct Volumetric CNN Regression. 
    :scroll: <a href="https://arxiv.org/abs/1703.07834"> paper </a> 
    :rocket: <a href="https://github.com/AaronJackson/vrn"> original_repo </a>
    :play_or_pause_button: <a href="https://www.youtube.com/watch?v=XWRRvUBN1wk"> video_youtube_here </a> </li>
</ul>

---