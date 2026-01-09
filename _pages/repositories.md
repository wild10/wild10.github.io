---
layout: page
permalink: /repositories/
title: Repositories
description: A collection of my open-source projects and code experiments.
nav: true
nav_order: 4
---

## Featured Projects

<div class="row">
    <!-- Project 1 -->
    <div class="col-sm-6">
        <div class="card mb-3">
            <!-- <img class="card-img-top" src="/assets/img/project1.png" alt="Project 1"> -->
            <div class="card-body">
                <h5 class="card-title">1. Traditional Machine Learning</h5>
                <p class="card-text">This is a collection of traditional ML learning projects,all included: Support Vector Machines (SVM),Hidden Markov Models (HMM),Naive Bayes,Decision Trees,Linear Regression,Logistic Regression, and k-Nearest Neighbors (k-NN).</p>
                <a href="https://github.com/wild10/machine-learning" class="btn btn-primary btn-sm">View Repo</a>
            </div>
        </div>
    </div>
    <!-- Project 2 -->
    <div class="col-sm-6">
        <div class="card mb-3">
            <div class="card-body">
                <h5 class="card-title">2. Deep Learning</h5>
                <p class="card-text">Description of your second most important project.</p>
                <a href="https://github.com/wild10/project2" class="btn btn-primary btn-sm">View Repo</a>
            </div>
        </div>
    </div>
    <!-- Project 3 -->
    <div class="col-sm-6">
        <div class="card mb-3">
            <div class="card-body">
                <h5 class="card-title">Project Name 3</h5>
                <p class="card-text">Description of your third most important project.</p>
                <a href="https://github.com/wild10/project3" class="btn btn-primary btn-sm">View Repo</a>
            </div>
        </div>
    </div>
    <!-- Project 4 -->
    <div class="col-sm-6">
        <div class="card mb-3">
            <div class="card-body">
                <h5 class="card-title">Project Name 4</h5>
                <p class="card-text">Description of your fourth most important project.</p>
                <a href="https://github.com/wild10/project4" class="btn btn-primary btn-sm">View Repo</a>
            </div>
        </div>
    </div>
</div>

## GitHub Stats

<div align="center">
  <!-- Trophies service is currently down, using stats card instead -->
  <!-- <img src="https://github-profile-trophy.vercel.app/?username=wild10&theme=flat&no-frame=true&margin-w=4" alt="GitHub Trophies" /> -->
  <img src="https://github-readme-stats-sigma-five.vercel.app/api?username=wild10&show_icons=true&theme=flat" alt="GitHub Stats" />
</div>

## All Repositories

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
