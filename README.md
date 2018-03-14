# trickortreat
routing with qgis presented through leaflet
Generate the best route for given waypoint
Range of options
Simply giving a few examples
Leaflet is just the interface. Need to find an actual routing service. Grass or Qgis
Way for gis people to find trick or treating spots.

Network analysis
jKstra
https://github.com/bbecquet/jKstra/blob/master/README.md
This is javascript for shortest path in graph. Very simple and seems you need to create your own graph
Grass’s version
http://grass.osgeo.org/programming6/dglib.html
c
Another Github library
https://github.com/kgeographer/topotime
Mapbox:Turf
https://www.mapbox.com/analysis/
js
QGIS
https://docs.qgis.org/2.18/en/docs/pyqgis_developer_cookbook/network_analysis.html
From polyline to graph
python

Post GIS
I’d like to take a weighted network graph and present the shortest route for that graph through leaflet. 

Everything will be local

Geojson weighted network analysis/routing
	 QGIS python
		Input and program settings
Have to load into database. Provider is a method of reading, not the data’s provider.
QgsLineVectorLayerDirector(vectorlayer,
 directionFieldId(where leftright/rightleft/both),
                                      directDirectionValue(“leftright”,
                                      reverseDirectionValue(rightleft),
                                      bothDirectionValue(both),
                                      defaultDirection(3)

possible property calculator, builder of graph requires start and end. So maybe needs to call this script every time?
Since start and end are the same, find largest value for x distance?
		create graph from geodata (usually polyline vector layer)
run graph analysis
use analysis results (for example, visualize them)
		How to output the calculated route/ how it’s output
	What format the Geojson needs to be in
Displaying the output via leaflet(not necessarily a 
	Customization alike typical webmap. 
Route Summary,
Information
Displaying calculation network

Polyline and graphs are separate? Seems like we need to load polylines into a graph. Maybe maps are graphs
Feature collections can’t be loaded into qgis if you set them with as a variable
Edge Values, or node values? Intersections are nodes. Roads are edges
