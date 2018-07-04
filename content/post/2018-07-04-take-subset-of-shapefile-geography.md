---
title: Take Subset of Shapefile Geography in QGIS
author: Carlos
date: '2018-07-04'
slug: take-subset-of-shapefile-geography-qgis
categories:
  - GIS
tags:
  - GIS
  - QGIS
  - Census
subtitle: ''
---

In the last post, we opened a shapefile that contained all census block groups in Texas in QGIS. In this post, I provide steps for taking a subset of a shapefile, particularly by keeping block groups located in Bexar County.

First, open the Texas shapefile and hover over the _zoom in_ icon, which is a magnifying glass with a plus sign inside

<br>
![](/post/shot-2018-06-27_19-47-24.png)

Then, zoom in on the region of Texas where Bexar County is located

<br>
![](/post/shot-2018-06-27_19-48-56.png)

Hover and click on the _open attribute table_ icon

<br>
![](/post/shot-2018-06-27_19-51-04.png)


Hover and click on the _select/filter features_ icon 

<br>
![](/post/shot-2018-06-27_19-51-34.png)

Input the Bexar County FIPS code 029 in the _COUNTYFP_ field, change the _Exclude Field_ option to _Equal to (=)_ and click on the _select features_ button

<br>
![](/post/shot-2018-06-27_19-56-11.png)

You will see that there are 1084 features (i.e. census block groups) in Bexar County

<br>
![](/post/shot-2018-06-27_19-56-45.png)

Hover and click on _Layer_ to open the _save as_ dialogue box. This will allow you to save the selected block groups in Bexar County as a separate shapefile layer. Make sure the _Save only selected features_ box is checked 

<br>
![](/post/shot-2018-06-27_19-58-25.png)

Afterwards, click on _Browse_ next to _File name_ and name the shapefile whatever you like. I named the file _bexar_county_shapefile.shp_

<br>
![](/post/shot-2018-06-27_19-58-39.png)

You have now saved and added the Bexar County census block groups as a separate shapefile!

<br>
![](/post/shot-2018-06-27_19-59-20.png)