---
layout: page
title: computer Vision projects
description:
img: assets/img/projects/1.jpg
redirect: 
importance: 1
category: work
---
During my Master program i study and reimplement some of the cool Deep learning projects.

---

### Video Classification 

Video classification is a critical task in the field of computer vision and machine learning, aimed at automatically categorizing videos into predefined classes based on their content.

<div class="row  justify-content-sm-center ">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/12.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/mZdsx-WhCwo" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/ivPULmZRb3U" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    The images show the implementation of video classification through the image classification method using Tensorflow and CNN.
</div>

<ul>
    <li>  Google Inception model to classify images. 
    :rocket: <a href="https://github.com/wild10/video_classification_modified_fimg_classification?tab=readme-ov-file"> original_repo </a>
    :play_or_pause_button: <a href="https://www.youtube.com/watch?v=mZdsx-WhCwo"> video_youtube_here </a> </li>
</ul>


---
### Action Recognition <span style="font-size: 16px;"> (Optical Flow paper reimplementation) </span>


<div class="row  justify-content-sm-center ">
    <div class="col-sm mt-3 mt-md-0">
        <a href="{{ site.baseurl }}/assets/img/projects/5.png" data-fancybox="project" title="Example Image" class="zoom" >
        {% include figure.liquid path="assets/img/projects/5.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </a>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/pNrzZKEyGtM" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/2hfm5tPyYEM" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The image in the left shows, the paper output and method and the videos in the right presents my own re-implementation for Action recognition Dataset.
</div>

Suitable feature representation is essential for performing video analysis and understanding in applications within the smart surveillance domain. In this projec, i re-implemented and ran the method called: called Optical Flow Co-occurrence Matrice probing its effectiveness for measuring flow patterns.

<ul>
    <li>haralick descriptor aproach "Optical Flow Co-occurrence Matrices: A novel spatiotemporal feature descriptor"
     :scroll:  <a href="https://ieeexplore.ieee.org/document/7899921"> paper_here </a> 	
     :package: <a href="https://www.csc.kth.se/cvap/actions/"> Dataset_here</a> 
     :rocket:  <a href=""> git_repo </a>
     :play_or_pause_button: <a href="https://www.youtube.com/watch?v=pNrzZKEyGtM"> video_youtube_here  </a> 
    </li>
    <li> Demo optical flow ActionRecognition using KTH :play_or_pause_button: <a href="https://www.youtube.com/watch?v=2hfm5tPyYEM"> video_youtube_here </a> </li>
</ul>


--- 
### 3D Image reconstruction

##### multiresolution hierarchies

Many tasks in geometry processing and physical simulation benefit from multiresolution hierarchies. In this project i aimed to re-implement and run this method to explore thi existing techniques such as surface mesh decimation, voxelization.The method constructs each next-coarsest level of the hierarchy using a sequence of decimation, flow. I also learnt using OPenGL,mesh with c++ and all the framework related to 3D analysis

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
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
        {% include figure.liquid path="assets/img/projects/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
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

#### Optical Character Recognition
 
 Image-based Automatic Meter Reading (AMR) hasbeen evaluated on images captured in well-controlled scenarios. However, real-world meter readings present unconstrained scenarios as other approaches focus in using previously well-selected images. Here we developed AMR using YoLO with real image scenarios with brith, low quality, and unknown scenarios for the Else company.

 <div class="row  justify-content-sm-center ">
    <div class="col-sm mt-3 mt-md-0">
        <a href="{{ site.baseurl }}/assets/img/projects/14.png" data-fancybox="project" title="Example Image" class="zoom" >
        {% include figure.liquid path="assets/img/projects/14.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </a>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/13.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/x8lLRVlOT1E" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    the images in the left show the detection of the display and digits, the vido show the demo implementation.
</div>

<ul>
    <li> Automatic Meter Reading in Unconstrained Scenarios. 
    :rocket: <a href="https://web.inf.ufpr.br/vri/publications/amr-unconstrained-scenarios/"> original_site </a>
    :play_or_pause_button: <a href=""> video_youtube_here </a> </li>
</ul>

--- 
### Object Detection using YOLO

In this project, I implemented a robust person detection system tailored for sports environments using YOLO. Leveraging real-time processing, this application accurately identifies and tracks individuals during dynamic gameplay, enhancing analysis and viewer engagement.



<div class="row  justify-content-sm-center ">
    <div class="col-sm mt-3 mt-md-0">
        <a href="{{ site.baseurl }}/assets/img/projects/18.png" data-fancybox="project" title="Example Image" class="zoom" >
        {% include figure.liquid path="assets/img/projects/18.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </a>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/-viWP8NUbQM" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


Key Features:

Real-Time Detection: Captures fast-paced action with minimal latency.
Custom Architecture: Optimized YOLO model fine-tuned for sports contexts.
Comprehensive Demo: Watch the detection in action here.
Explore the full project on my GitHub repository for detailed architecture and implementation insights!

---
### images segmentation using SAM

<div class="row  justify-content-sm-center ">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/16.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/mZdsx-WhCwo" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

---