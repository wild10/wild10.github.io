# My Personal Website

Welcome to My Awesome Website wild10.git.io ! This project is a simple web application built with a template all the credits to [Al-Folio Theme](./README_tuto.md) nicely edited by myself.

## Table of Contents

- [About](#About)
- [Publications](#Publications)
- [Projects](#Porfolio)
- [Repositories](#Repositories)
- [CV](#CV)
- [Teaching](#Teaching)

## Features

- About me and my interest.
- Porfolio with NLP, CV & ML projects described.
- My CV and experiences so far.
- Research Experience & Taslks and other interesting things.

## Installation & Run

to get a local copy of the web, follow these steps:

create and virtual env with basic python.
```bash
sudo apt install imagemagick
# Comandos de instalación
source /home/wilderd/anaconda3/bin/activate
# activate the env
conda activate fmo_yolo
# give super user
sudo bundle exec jekyll serve
```

## Run with docker

first we need to create the container, and then we run it. Altough we can use the same command to build and run the container. we needed to fix the docker file: to use ruby:3.1 instead of latest.

```bash
   # crear imagen docker
   docker compose build --no-cache

   # run the container
   docker compose up -d
```

after running we are going to see that we have a container running using:

```bash
   # show running containersS
   docker ps
```
check the website at: http://0.0.0.0:8080/

