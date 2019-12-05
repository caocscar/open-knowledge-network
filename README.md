# open-knowledge-network
1. How complete is HPMS (and its underlying referencing systems) nationally? How open is it across states?

There are shapefiles for all 50 states, DC and PR. There is also a national shapefile which has a subset of the roads in the state files.

2. How similar are the road segments in OSM and Framework (as an example)?

Framework road segments are usually defined by intersections at its endpoints. OSM road segments are longer than that and can pass through multiple intersections.

3. What would be involved in mapping between these two systems?

OSM road segments consists of nodes. Nodes are GPS points that define the road segment. There are nodes in the road segments that define intersections. 
- We would have to locate the intersection nodes in OSM. 
- Then we could do map matching using the endpoints of road segments to intersection nodes in OSM (or vice versa)

Fortunately, Scott Bogard, has done item one already. He has constructed a table of all intersection nodes in the continental USA. It is located on the server `tri.esg.gm1` in the database `OSM2019`.
