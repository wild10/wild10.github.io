---
layout: page
title: NLP projects
description: A small set of Natural Language Processing projects.
img: assets/img/projects/2.jpg
importance: 2
category: work
giscus_comments: false #true
---

---
### Text Classification
##### 1. Aggressive Language identification using Vocabulary Graph Convolutional Neural Network

Developed a robust model for detecting offensive and hate speech in text using Graph Neural Networks (GNNs). I represented vocabulary as a graph to capture word relationships, enhancing contextual understanding. Implemented the solution in PyTorch, utilizing various frameworks for efficient data processing and model training. The project achieved high accuracy in identifying harmful language.

<div style="text-align: justify">
    <div class="row  justify-content-sm-center ">
        <div class="col-sm-8 mt-3 mt-md-0">
            <a href="{{ site.baseurl }}/assets/img/projects/nlp/1.png" data-fancybox="project" title="Example Image" class="zoom" >
                {% include figure.liquid path="assets/img/projects/nlp/1.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </a>
        </div>
    </div>
</div>
<div class="caption">
    The results of Aggressive detection using VGCN f1-score, *means our developed system model.
</div>

Read more
<ul>
    <li> 
        VGCN for Aggressive detection |
        :scroll: <a href="https://link.springer.com/chapter/10.1007/978-3-030-91699-2_25"> paper_here </a> 
        :rocket: <a href="https://github.com/wild10/vgcn_bert_mxa3t">git_repo</a>
    </li>
</ul>
--- 

##### 2. Sentiment Analysis for Spanish (Peru) using SVM

I developed a machine learning project using Support Vector Machines (SVM) for text classification. I collected real-time tweets from Twitter to train the model, focusing on sentiment analysis. The project demonstrated SVM's effectiveness in classifying textual data accurately.

<div style="text-align: justify">
    <div class="row  justify-content-sm-center ">
        <div class="col-sm-4 mt-3 mt-md-0">
            <a href="{{ site.baseurl }}/assets/img/projects/nlp/4.png" data-fancybox="project" title="Example Image" class="zoom" >
                {% include figure.liquid path="assets/img/projects/nlp/4.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </a>
        </div>
    </div>
</div>
<div class="caption">
    General Pipeline followed to implement SVM for Sentyment analysis case study.
</div>

Read more
<ul>
    <li> 
        Analisis masivo de datos en twitter para identificacion de opinion 
        :scroll: <a href="https://repositorio.unsaac.edu.pe/handle/20.500.12918/5252">thesis_online_repor </a>
        :rocket: <a href="https://github.com/wild10/twitterSentimentAnalisis/blob/master/test.ipynb">git_repo</a>
    </li>
</ul>

--- 
---
### Text Generation

#### 1. Quechua Indigenous Lyrics Generation using LSTM.

Developed a text generation model for the Quechua language using LSTM networks. Collaborated with a team to create the dataset, then successfully training the model to generate coherent text lyrics of songs. This project aims to promote and preserve Quechua, enhancing its accessibility in digital formats and supporting cultural heritage.

<div class="row  justify-content-sm-center ">
    <div class="col-sm mt-3 mt-md-0">
        <a href="{{ site.baseurl }}/assets/img/projects/nlp/17.png" data-fancybox="project" title="Example Image" class="zoom" >
            {% include figure.liquid path="assets/img/projects/nlp/17.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </a>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/COpDxR9u9fQ" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    the video in the right shows the demo of the Quechua lyrics generation.
</div>

Read more
<ul>
 <li>Generación automática de letras de canciones usando redes neuronales recurrentes para el quechua
  :scroll: <a href="https://repositorio.unsaac.edu.pe/handle/20.500.12918/7276"> thesis_online_repor </a>
  :rocket: <a href="https://github.com/wild10/Quechua_lyrics_generation"> git_repo </a>
 </li>
</ul>

---
### Speech Recognition

#### 1. A Comparison Study of Speaker Identification models

This project compares three machine learning models: Gaussian Mixture Model (GMM), Hidden Markov Model (HMM), and Support Vector Machines (SVM). Using the same MFCC features, HMM and GMM achieved about 94% accuracy on 100 audio recordings. SVM reached around 90% accuracy for classifying 2-5 individuals but performed poorly with more classes.

Read more
<ul>
 <li>
  :rocket: <a href="https://github.com/wild10/Comparation_Study_SR"> git_repo </a>
 </li>
</ul>



