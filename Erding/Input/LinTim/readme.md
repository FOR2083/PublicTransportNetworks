# LinTim Format
All LinTim input files can be opened with a text editor. The input contains the following files to describe the network supply:
-	Edge.giv
-	Load.giv
-	OD.giv
-	Stops.giv

Each file contains a header describing the column content. An additional explanation of the column is given below for each input file.

## Edge.giv
-	edge-ID: unique ID for each edge between two stops
-	left-stop: ID of the “left” stop to represent directed and undirected networks. Undirected networks do not need the information of the opposite direction. 
-	right-stop: ID of the “right” stop
-	length: length of the edge in kilometer
-	min travel time: minimum travel time to pass the edge with the highest allowed speed
-	max travel time: maximum travel time to pass the edge with the lowest accepted speed 

## Load.giv
The Load.giv file provides information for loads on edge level.
-	edge-ID: unique ID for each edge
-	load: passenger load on edges
-	lower-frequency: The lower-frequency indicates the minimum of required service runs per hour to serve the loads on edges. The lower frequency depends on the vehicle capacity.
-	upper-frequency: The upper-frequency indicates the maximum of service runs per hour on edges. The default value is set to 20.

## OD.giv
The OD.giv file provides information for the demand on origin-destination level. 
-	left-stop-ID: ID of the “left” stop
-	right-stop-ID: ID of the “right” stop
-	customers: It represent the amount of location changes in the network starting the trip at the origin and terminating the trip at the destination stop. 

## Stops.giv
-	stop-id: unique ID for each stop
-	short-name: The short-name corresponds to the unique numbering in VISUM
-	long-name: The long-name describes the stop.
-	x-coordinate: No explicate coordinate system is defined. 
-	y-coordinate: No explicate coordinate system is defined.

