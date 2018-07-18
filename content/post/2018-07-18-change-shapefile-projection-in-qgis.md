---
title: Change Shapefile Projection in QGIS
author: Carlos
date: '2018-07-18'
slug: change-shapefile-projection-in-qgis
categories:
  - GIS
  - Software
tags:
  - GIS
  - QGIS
subtitle: ''
---

After creating our Bexar County shapefile, by taking the subset of the Texas shapefile (see [here](https://carlosvalenzuela.netlify.com/post/take-subset-of-shapefile-geography-qgis/)), I wanted the shapefile to have a different projection, especially one that is good for showing smaller geographies, such as counties. For Bexar County, the projection I want to use is UTM.

First, open QGIS and click on the EPGS icon on the bottom far right corner.

![](/post/shot-2018-07-18_10-10-35.png)

<br>

Enable on the fly projection (i.e. make sure box is checked), select NAD27/UTM zone 14N, and click OK (or press ENTER)

![](/post/shot-2018-07-18_10-38-13.png)

<br>

Open the Bexar County shapefile we created (again from previous post)

![](/post/shot-2018-07-18_10-39-05.png)

As you can see, the shapefile already looks different. This is because we initially set the project with the projection we wanted. In order for us to to have the shapefile with this projection for future use, we must save it.

Right-click on the shapefile (bottom-left panel) and select save Layer as.

Name the shapefile. You can do this by clicking on _Browse_, choosing location and name. I ended up just adding _UTM_ to the shapefile name. 

Make sure that CRS UTM is selected. 

Click OK.

![](/post/shot-2018-07-18_10-40-07.png)

We have just changed and saved our shapefile with a new projection!

![](/post/shot-2018-07-18_10-40-44.png)


