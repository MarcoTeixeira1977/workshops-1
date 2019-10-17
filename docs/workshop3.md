---
layout: "default"
title: "Workshop description #3 - Inspire Helsinki 2019"
description: "Material for workshops"
page: "workshop3"
---
# OGC API Features: enhanced usability for existing WFS services

In this workshop we will set up "OGC API - Features" service which will provide a simple RESTful API and additional output formats like GeoJson, HTML and JSON-LD. These representations are created on the fly using live data from the existing WFS service(s).

The emerging OGC API standards are an important step to make spatial data more easily accessible using open standards and in Web APIs. OGC API Features, formerly known as "WFS 3.0" (it started as a revision of the OGC WFS standard) has been leading this process. After two years of intensive implementation and testing the first part of OGC API Features has been approved and [published by OGC](http://docs.opengeospatial.org/is/17-069r3/17-069r3.html). This [OGC blog post](https://www.opengeospatial.org/blog/2996) has additional information about OGC API.

In this workshop you will learn:
* how OGC API Features differs from WFS and why;
* how to set up a Web API facade supporting OGC API standards in front of an existing WFS using ldproxy;
* how your Web API makes the data more accessible and easier to use for both developers and users;
* how to update the configuration of your Web API to further improve usability.

[ldproxy](https://github.com/interactive-instruments/ldproxy) is an open source implementation for geospatial Web APIs supporting the OGC API standards. One option is to use ldproxy as a proxy in front of existing WFS services and provides a simple Web API and additional output formats like GeoJSON and HTML. These representations are created on the fly using live data from the WFS.

In the workshop we will be using a development version of ldproxy 2.0, which is expected to be released late 2019 or early 2020. The reason for using the development version is that it has aready been updated to conform to the published standard and it supports additional capabilities.

# What skills are requried?

We will demonstrate all steps in detail and use live services to explain and demonstrate the OGC API concepts. Basic knowledge of OGC WFS, JSON and GeoJSON will help, but is not essential.

You are encouraged to set up your own Web API during the workshop and follow the steps hands-on. For this, you will need to deploy ldproxy on your maschine. The easiest way to do this is to use Docker, which must be installed on your computer before the workshop - see the next section.

# Preparation before the workshop

This is only required, if you want to play with your own Web API on your notebook during the workshop.

As mentioned above the easiest way to deploy ldproxy on your machine is to use Docker. If you are new to Docker, have a look at the [Docker Documentation](https://docs.docker.com/). Getting started with Docker is straightforward on Linux or macOS. On Windows, you are more likely to encounter issues depending on your local setup and permissions. For example, you may need to open ports in your firewall.

Once Docker is up and running, you can deploy ldproxy on your machine.

1. Create a directory for the ldproxy data on your machine (e.g. `C:/ldproxy_data` or `~/ldproxy_data`). Make sure it is a directory that is shared with Docker.

2. Download and start ldproxy on port 80: `docker run --name ldproxy -d -p 80:7080 -v C:/ldproxy_data:/ldproxy/data iide/ldproxy:t15`. This downloads the latest ldproxy docker container from the t15-development branch.

3. Once the docker container has been downloaded, ldproxy will start. After a minute or so open `http://localhost/` in your browser and you should be redirected to `http://localhost/manager/#/services` and see the ldproxy manager.

We continue to update the current ldproxy development branch before the workshop, so if you have deployed ldproxy on your machine before 21 October 2019, please check before the workshop, if a newer version of the [t15 branch of ldproxy is available on docker Hub](https://hub.docker.com/r/iide/ldproxy/tags?name=t15). In this case, follow the clean-up instructions below and redeploy ldproxy using the steps above.

See also the section [Deploying ldproxy](http://interactive-instruments.github.io/ldproxy/manual/00-deployment.html) in the ldproxy documentation.

# Clean up after the workshop

To remove the installation and the files again:
1. Delete the ldproxy data directory e.g. `C:/ldproxy_data` or `~/ldproxy_data`).
2. Stop ldproxy using `docker stop ldproxy` and then remove the container using `docker rm ldproxy`.

# Sample WFS services

If you have a URL of a public WFS 2.0 with data that you are interested in, great, but here is a short list of some sample WFS URLs that you can use, too.

* [http://www.wfs.nrw.de/geobasis/wfs_nw_alkis_vereinfacht?SERVICE=WFS&REQUEST=GetCapabilities](http://www.wfs.nrw.de/geobasis/wfs_nw_alkis_vereinfacht?SERVICE=WFS&REQUEST=GetCapabilities)  
Cadastral dataset from North-Rhine Westphalia in Germany. This is the same WFS 2.0 that is available using an older version of ldproxy at https://www.ldproxy.nrw.de/kataster.

* [http://services.rce.geovoorziening.nl/landschapsatlas/wfs?service=WFS&request=GetCapabilities](http://services.rce.geovoorziening.nl/landschapsatlas/wfs?service=WFS&request=GetCapabilities)  
Various landscape data from the Netherlands.

* [https://geodienste.hamburg.de/HH_WFS_EMobility?SERVICE=WFS&REQUEST=GetCapabilities](https://geodienste.hamburg.de/HH_WFS_EMobility?SERVICE=WFS&REQUEST=GetCapabilities)  
Charging stations for electric cars in the city of Hamburg, Germany.

* [http://geoserver.ymparisto.fi/geoserver/wfs?SERVICE=WFS&REQUEST=GetCapabilities](http://geoserver.ymparisto.fi/geoserver/wfs?SERVICE=WFS&REQUEST=GetCapabilities)  
Various INSPIRE data from SYKE in Finland.

* [https://geodata.nationaalgeoregister.nl/inspireadressen/v2/wfs?SERVICE=WFS&&REQUEST=GetCapabilities](https://geodata.nationaalgeoregister.nl/inspireadressen/v2/wfs?SERVICE=WFS&&REQUEST=GetCapabilities)  
Address data from the Netherlands.

* [http://sg.geodatenzentrum.de/wfs_dlm1000?SERVICE=WFS&REQUEST=GetCapabilities](http://sg.geodatenzentrum.de/wfs_dlm1000?SERVICE=WFS&REQUEST=GetCapabilities)  
1:1000000 topographic data from Germany.

* [http://data.isric.org/geoserver/wosis_latest/wfs?SERVICE=WFS&REQUEST=GetCapabilities](http://data.isric.org/geoserver/wosis_latest/wfs?SERVICE=WFS&REQUEST=GetCapabilities)  
World Soil Information Service (WoSIS) data.

# Other information

* Organizers of the workshop: 
    * Clemens Portele, [interactive instruments](https://www.interactive-instruments.de/en/)
    * Jari Reini, [National Land Survey of Finland](https://www.maanmittauslaitos.fi/en)
* Duration of the workshop: 1.5 hours
* Event programme [https://www.inspire-helsinki-2019.fi/programme](https://www.inspire-helsinki-2019.fi/programme)
