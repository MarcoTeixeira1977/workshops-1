---
layout: "default"
title: "Workshop description #3 - Inspire Helsinki 2019"
description: "Material for workshops"
page: "workshop3"
---
# OGC API Features: enhanced usability for existing WFS services

In this workshop we will set up "OGC API - Features" service which will provide a simple RESTful API and additional output formats like GeoJson, HTML and JSON-LD. These representations are created on the fly using live data from the existing WFS service(s).

The emerging OGC API standards are an important step to make spatial data more easily accessible using open standards and in Web APIs. OGC API Features, formerly known as "WFS 3.0" (it started as a revision of the OGC WFS standard) has been leading this process. After two years of intensive implementation and testing the first part of OGC API Features is now in the approval process in OGC and should be available as the first OGC API standard before the Inspire Helsinki 2019 event. This [OGC blog post](https://www.opengeospatial.org/blog/2996) has additional information about OGC API.

In this workshop you will learn
* how OGC API Features differs from WFS and why;
* how to set up a Web API facade supporting OGC API standards in front of an existing WFS using ldproxy;
* how your Web API makes the data more accessible and easier to use for both developers and users;
* how to update the configuration of your Web API to further improve usability.

[ldproxy](https://github.com/interactive-instruments/ldproxy) is an open source implementation for geospatial Web APIs supporting the OGC API standards. One option is to use ldproxy as a proxy in front of existing WFS services and provides a simple Web API and additional output formats like GeoJSON and HTML. These representations are created on the fly using live data from the WFS.

# What you should bring

We will demonstrate all steps in detail and use live services to explain and demonstrate the OGC API concepts. Basic knowledge of OGC WFS, JSON and GeoJSON will help, but is not essential.

You are encouraged to set up your own Web API during the workshop and follow the steps hands-on. To do this, you need Docker on your notebook. If you are new to Docker, have a look at the [Docker Documentation](https://docs.docker.com/). If you have a URL of a public WFS 2.0 with data that you are interested in, great, but we will also provide sample URLs for you to play with.


# Other information

* Organizers of the workshop: [interactive instruments](https://www.interactive-instruments.de/en/), [National Land Survey of Finland](https://www.maanmittauslaitos.fi/en)
* Duration of the workshop: 1.5 hours
* Event programme [https://www.inspire-helsinki-2019.fi/programme](https://www.inspire-helsinki-2019.fi/programme)
