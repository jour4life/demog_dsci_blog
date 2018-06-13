---
title: Install QGIS with Anaconda
author: Carlos
date: '2018-06-12'
slug: install-qgis-with-anaconda
categories:
  - GIS
  - Software
tags:
  - QGIS
  - GIS
  - Python
subtitle: ''
---

In grad school, I enjoyed working on spatial analyses using R and ArcMap. Since I am no longer and grad school, and have no appetite in spending hundreds of dollars to use software, I would like to get more comfortable using [QGIS](www.qgis.org), which is free, open source, and available on Windows, Mac, and Linux.

Recently, I installed [Bodhi](https://www.bodhilinux.com/) Linux on my old laptop. It's a lightweight Linux distro, which is useful since my laptop is already 8 years old. After installing Bodhi, I (of course) installed [R](https://cran.r-project.org/) and [Anaconda](https://conda.io/docs/user-guide/install/download.html) to conduct my everyday analytical/data science activities. I then attempted to install QGIS as per the web sites instructions and kept running into errors. I had never encountered difficulties installing QGIS on other Linux distros. Since QGIS uses/depends on Python quite a bit, it could be that something messed up along the way after installing Anaconda. Luckily, I found a way to install QGIS using Anaconda.

These are the steps I took to install QGIS using Anaconda:

- Create a new environment, installing Python 2.7 

```console
user@console: ~$ conda create --name gis_env python=2.7

```

- Add the conda-forge channel 

```console
user@console: ~$ conda config --add channels conda-forge

```

- Activate the newly created environment

```console
user@console: ~$ source activate gis_env

```

- Install QGIS

```console
user@console: ~$ conda install qgis

```

- Open QGIS

```console
user@console: ~$ qgis

```

Now you're ready to use QGIS!

![](/post/2018-06-12-install-qgis-with-anaconda_files/qgis_screenshot.png)