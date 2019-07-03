---
layout: "default"
title: "Workshop description #1 - Inspire Helsinki 2019"
description: "Material for workshops"
page: "workshop1"
---
# INSPIRE, WFS3 and HALE Support in GeoServer: where are we?

GeoServer is a well-established multiplatform, open source server providing a variety of OGC services, including WMS (view services), WFS and WCS (download and edit services) as well as WPS (spatial data processing services). 
 
Amongst the open source GIS web servers, GeoServer is well known for the ease of setup, the web console helping the administrator to configure data and services, the variety of OGC services available out of the box, as well as the rich set of data sources that it can connect to (open source, such as PostGIS as well as proprietary, such as Oracle or ECW raster). 
 
Most WFS systems available online today trade (very) simple features, often a single geometry with a set of attributes exposed on the net for querying, reprojection and download. However, the world of WFS and GML does not stop there, the standard also foresees complex features, where each feature is an information tree, with lists, sub-features, and links to other features. GeoServer provides support for those via the app-schema plugin, which can map a heterogeneous set of simple features, coming from different data sources, onto a set of complex features described by a well-known application schema. 
 
Meanwhile, the new version of the WFS protocol, WFS 3.0 is being shaped by OGC in a collaborative manner. WFS 3.0 core protocol is geared towards the web and simplicity: dominated by (Geo) JSON representations, only supports WGS84 in and out, it’s schema-less, and has limited filtering and paging abilities. Everything else you are used to see in WFS 1.1 or WFS 2 will be delivered as extensions to the core, that implementers can decide to implement, or not. The approach is similar to WCS, small core and various extensions, helps getting started implementing the protocol and it’s a lot of help when building custom servers. GeoSolutions has been involved in this effort with OGC since the beginning through hackathons, Interoperability Testbeds and so on. 
 
The workshop will provide a hands-on introduction to the basic GeoServer concepts, as well as usage and configuration, with particular attention to the setup of INSPIRE compliant services with a demonstration set of data in various formats, both raster and vector. We will show how complex features are configured and setup in GeoServer, the abilities and limitations of the app-schema module, as well as recent advances in producing a configuration starting point with the help of HALE mapping tool. Eventually we will cover WFS 3 support in GeoServer in terms of its current status and the expected evolutions. 

# Requirements for participants

* Basic knowledge of GeoServer 
* Basic knowledge of WFS 3 
* Basic Knowledge of HALE 
* Not being afraid of GML!

# Other information

* Organizer of the workshop: [https://www.geo-solutions.it/](GeoSolutions SAS)
* Duration of the workshop: 3 hours
* Event programme [https://www.inspire-helsinki-2019.fi/programme](https://www.inspire-helsinki-2019.fi/programme)
