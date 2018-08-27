# How JupyterLab and widgets enable interactive analysis of the Earth's past, present, and future

Tyler Erickson: Google (He's a Snow Hydrologist)

>The Earth is rapidly changing, and this change has numerous important environmental and societal impacts. There is a strong need to understand these changes at a global scale in high resolution so that we might reverse or adapt to them.

[Google Earth Engine](https://earthengine.google.com/)

[Notebook GitHub](https://github.com/tylere/ee-jupyter-examples)

[Earth Engine Summit](http://g.co/earth/eeus2018)

Colaboratory - Free Hosted Jupyter Notebook Environment

Tyler helps NGOs and groups around the world to approach geospatial data science for humanitarian reasons

Topics include:

* Trends in adoption of Jupyter technologies at Earth science conferences data and by Earth science data and information providers
* How to combine multiple Jupyter widgets in JupyterLab to interactively explore and analyze high-dimensional data stored on remote platforms
* Case studies of using Jupyter widgets for Earth science data analysis, such as analyzing land-cover change models and exploring projections of future climate conditions

While the case studies will use Google’s Earth Engine platform, the techniques demonstrated are applicable to most remote geospatial platforms that provide API access.

## Spatial is Special - Geospatial Data Quirks
e.g. lat, lon, pressure, creation time, forcast time, model forcing parameters

Distance/proximity is important "Cant See it, look around it"

The data is NOT static at all

Landsat - satellite ~450 GB per scene, one scene per 45 seconds for around the last 40 years

1970 - $15
1980 - $6000
1990 - $600
2009 - free - Creation of Earth Engine

Landset scenes are **messy**, a lot of post processing by NASA is required to polish it up

ipyleaflet is a widget for mapping
bqplot 2d time spanning data visualization

## Earth Engine

it is a web api for a lot of geospacial datasets

* \>10 Petabytes large
* \>200 public datasets
* \>5000 new images a day
* \>5 million images

Javascript and Python api






