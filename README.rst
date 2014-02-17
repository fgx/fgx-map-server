fgx-map-server
==============================

Mapnik server for fgx project.
Uses postgis database from fgx-navdata project

===============
Install
===============

Mapnik
---------------------------------
Clone mapnick
git clone https://github.com/mapnik/mapnik.git

Install OGCServer server
git clone https://github.com/mapnik/OGCServer.git
cd OGCServer
sudo python setup.py install

run the server
on ubuntu 
    /usr/local/bin/ogcserver ./resources.xml 
on debian
    /usr/??local/bin/ogcserver ./resources.xml 

point your maps at
http://localhost:8000/?LAYERS=Landmass&TRANSPARENT=True&FORMAT=image%2Fpng&SRS=EPSG%3A3857&SERVICE=WMS&VERSION=1.1.1&REQUEST=GetMap&STYLES=&BBOX=2504688.5425,2504688.5425,3757032.81375,3757032.81375&WIDTH=256&HEIGHT=256


