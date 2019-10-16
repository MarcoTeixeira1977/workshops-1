---
layout: "default"
title: "Workshop description #2 - Inspire Helsinki 2019"
description: "Material for workshops"
page: "workshop2"
---
# Building Web and Mobile Friendly Applications on top of INSPIRE data services, recent updates and real time streams

This workshop will look at how to build some practical web and mobile applications using a stack that includes both traditional INSPIRE data sources and a variety of real time and new API sources such as OpenAPI and WFS3. 
 
The goal will be to demonstrate a results based approach, where the basic output requirements are defined, and then a sequence of data sources and services are integrated to meet those requirements. 
 
A flood impact application will be developed in the context of the workshop, with templates, instructions and cloud instances made available to all participants. The scenario will integrate basemap information from INSPIRE infrastructure and flood hazard themes combined with recent updates and real time data from available SOS, IoT, SensorThings API and other available sources. The goal will be to produce a basic dashboard and supporting reports that depict the status and impact of a developing flood event, with key indicators summarized in chart, tabular and map form. 
 
The stack is expected to include the following components: 
* Mediating service that reads INSPIRE WFS2, WCS, IoT, OGC SensorThings API, and WMS and updates a OGC Geopackage staging database 
* The OGC Geopackage is then used to generate WFS3 / OGCAPI REST services with JSON, GeoJSON encodings 
* Browser and mobile web map clients that use leaflet, vector tiles or equivalent 
* Options for off-line viewing (pdf, html etc) 
 
Through the course of the workshop we will begin with a basic template for each subsystem and show how new data sources or services can be added or published through that subsystem. 
 
We will also discuss or examine how web / mobile clients can submit or push data to INSPIRE workflows. 
 
In the end participants will have a working web application that they can access from their web browser or mobile device. They will also have learned how to use FME to support data transformation, integration and conversion of INSPIRE data with alternate encodings such as Geopackage, GeoJSON and next generation OGC services such as WFS3 and Vector Tiles.

# Requirements for participants

Attendees are encouraged to bring their own laptops or may work with others. Ideally attendees should have downloaded the most recent release of FME ahead of time from [safe.com/downloads](https://www.safe.com/downloads). Free licensing will be made available during the workshop. We also recommend a good text / xml editor such as [Notepad++](https://notepad-plus-plus.org/).

# Other information

* Organizers of the workshop: 
  * Dean Hintz, [Safe Software](https://www.safe.com/)
  * Sören Dupke, [con terra](https://con-terra.com/)
* Duration of the workshop: 3 hours
* Event programme [https://www.inspire-helsinki-2019.fi/programme](https://www.inspire-helsinki-2019.fi/programme)
