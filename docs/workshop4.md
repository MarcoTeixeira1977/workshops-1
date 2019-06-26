---
layout: "default"
title: "Workshop description #4 - Inspire Helsinki 2019"
description: "Material for workshops"
page: "workshop4"
---
# 1st part: Event-Driven INSPIRE

Many applications rely on the timely delivery of data. This can comprise: 
 
* Monitoring applications, which continuously check certain environmental parameters (e.g. air quality) or risks (e.g. flooding risk based on water level measurements). 
* Mapping applications of dynamic properties (e.g. radar images, flight/ship tracking)
* Complex analysis workflows which require up-to-date satellite imagery as input
* Catalogue clients that shall notify users about new available data sets or updates to existing data sets 
 
However, the existing INSPIRE approaches for data delivery are based on pull-style communication. That means that clients connect to servers and check if new data is available. With new communication protocols and specifications that are currently becoming available, push/event-based data delivery becomes a new option. 
 
This promises two important benefits: 
 
a) Faster delivery of information: With a push-based communication pattern the delivery of data can happen as soon as new data sets are available. 
 
b) Reduction of server and network load: Currently, clients have to regularly query servers to check if new or updated data is available. If new data is directly delivered as soon as it is available, the server load created by continuously polling clients can be avoided. 
 
Within this workshop we would like to provide an introduction into technologies and standards (e.g. MQTT, AMQP, OGC Publish/Subscribe, OGC SensorThings API) that may help to enable event-driven communication patterns within INSPIRE. Besides introductory presentations, this will also comprise demonstrations of practical applications (e.g. the German research project WaCoDiS) and potentially hands-on experiences with selected technologies (e.g. accessing near real-time data streams delivered through MQTT brokers).

# 2nd part: Exchange of experience of vector tile service: pros and cons

A vector tile is a vector representation of geographic data covering a spatially contiguous and rectangular extent. They are similar to raster (image) map tiles in their intent, namely to provide support to fast map services which can take advantage of pre-rendering, caching and concurrent requests. They are different because instead of providing a pre-styled fixed image depiction of the geographic data, they are a vector representation which can be manipulated, e.g. styled, client-side. It is important to highlight that they are a representation of data intended for visualization, and thus they belong to view services and not to download services; the underlying data, i.e. the geographic features, will be selected, combined, simplified and cropped to generate small vector tiles that can be quickly delivered to relatively simple client devices and applications, where they will be styled. 
 
From the point of view of the service interface, vector tiles are no different to image tiles, they just happen to be in a different format (i.e. instead of PNG, they may be encoded in GeoJSON or Protocol Buffers). This means that they can be served through any view service interface that supports raster tiles (e.g. OGC WMTS, TMS or WMS-C), although the server which implements those interfaces must provide at least certain support for them. 
On this presentation, I'm going to show the process to create the vector tile service, from the data analysis to the service optimizing 

Participants can try the clients and vector tile service of the presentation.

# Requirements for participants

There are no specific requirements. Generally an understanding of Spatial Data Infrastructures and an interest in new technologies will be helpful. For trying out technology demos, participants should bring their laptop.

# Other information

* Organizer of the workshop: 52°North & Center of National Geographic Information, Spain
* Duration of the workshop: 1.5 hours
* Event programme [https://www.inspire-helsinki-2019.fi/programme](https://www.inspire-helsinki-2019.fi/programme)
