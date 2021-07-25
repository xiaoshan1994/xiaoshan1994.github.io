---
title: "RP Project"
date: 2021-05-26T10:10:16+02:00
tags:
- research proposal
Categories:
- Research
---

## Measuring in Arc-Seconds
[The source link](https://www.esri.com/news/arcuser/0400/wdside.html)
* USGS: United States Geological Survey. <br>
* DEM: Digital elevation model [Wiki search](https://en.wikipedia.org/wiki/Digital_elevation_model#:~:text=A%20digital%20elevation%20model%20(DEM,to%20a%20discrete%20global%20grid)

Some USGS DEM data is stored in a format that utilizes three, five, or 30 arc-seconds of longitude and latitude to register cell values. The geographic reference system treats the globe as if it were a sphere divided into 360 equal parts called degrees.
Said differently, an arc-second represents the distance of latitude or longitude across the earth's surface with the angle of one second.

At the equator, an arc-second of longitude approximately equals an arc-second of latitude, which is 1/60th of a nautical mile (or 101.27 feet or 30.87 meters). Arc-seconds of latitude remain nearly constant, while arc-seconds of longitude decrease as one moves toward the earth's poles. At 49 degrees north latitude, along the northern boundary of the Concrete sheet, an arc-second of longitude equals 30.87 meters * 0.6561 (cos 49°) or 20.250 meters.

[A comparison between two raster datasets from USGS DEM](https://pro.arcgis.com/en/pro-app/latest/tool-reference/conversion/how-dem-to-raster-works.htm)

## About spatial resolution (cell size of raster data)

![image](https://user-images.githubusercontent.com/65668613/119641779-4c17fe00-be1a-11eb-8620-8047bee53357.png)

The level of detail (of features/phenomena) represented by a raster is often dependent on the cell (pixel) size, or spatial resolution, of the raster. The cell must be small enough to capture the required detail but large enough so computer storage and analysis can be performed efficiently. More features, smaller features, or a greater detail in the extents of features can be represented by a raster with a smaller cell size. However, more is not often better. Smaller cell sizes result in larger raster datasets to represent an entire surface; therefore, there is a need for greater storage space, which often results in longer processing time.

You must balance your application's need for spatial resolution with practical requirements for quick display, processing time, and storage.

The following factors should be considered when specifying the cell size:

* The spatial resolution of the input data
* The application and analysis that is to be performed
* The size of the resultant database compared to disk capacity
* The desired response time

[See also ](https://desktop.arcgis.com/en/arcmap/latest/manage-data/raster-and-images/cell-size-of-raster-data.htm) Types of resolution and Spatial resolution versus scale.

[6.A. Grid Spacing and Resolution](https://www.ngdc.noaa.gov/mgg/topo/report/s6/s6A.html)
