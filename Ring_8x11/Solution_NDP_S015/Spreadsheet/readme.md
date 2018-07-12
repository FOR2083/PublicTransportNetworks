# Spreadsheet Output Format
The output spreadsheet contains the following tables to describe the network supply:
-	summary
-	attribute
-	node
- 	link
-	zone
-	stop
-	odpair
-	lineroute
-	linerouteitem
-	vehjourney
-	vehjourneyitem
-	image	

## summary
-	the sheet lists typical characteristics of the network for input values
-	two pictures are embedded to show the network instrastruktur and the demand situation  

## attribute
-	the list describes the available attributes for each network object
-	each attribute is characterized by networkobject name, VISUM attribute name, description, unit and datatype

## node
-	the list is given in VISUM format to provide a reimport to VISUM
-	each node is characterized by: number, code, name, xcoord, ycoord

## link
-	the list is given in VISUM format to provide a reimport to VISUM
-	each link is haracterized by: number, from node number, to noden number, length, maximum privat transport speed limit, public transport travel time
-	assignment results for each link is characterized by: public transport volume during the peak hour, public transport capcity during the peak hour, public transport saturation during the peak hour

## zone
-	the list is given in VISUM format to provide a reimport to VISUM
-	each zone is characterized by: number, code, name, xcoord, ycoord

## stop
-	the list is given in VISUM format to provide a reimport to VISUM
-	each stop is characterized by: number, code, name, xcoord, ycoord

## odpair
-	the list is given in VISUM format to provide a reimport to VISUM
-	each origin-destination-pair is characterized: by from node number, to node number, sum of the total demand, sum of privat transport demand, sum of public transport, sum of public transport during peak hour
-	assignment results for each odpair is characterized by: in-vehicle time, walk time at stops, transfer waiting time at stops, number of transfers between stops, perceived journey time according to the perceived journey time calcualtion (description of the instance), perceived journey time with minimum perceived journey time (passengers take shortest path)

## lineroute
-	the list is given in VISUM format
-	the list summerizes the skims of each line route
-	each line route is characterized by: line name, line route name, direction code, length, sum of the link run time, number of departures (trip) during the peak hour.

## linerouteitem
-	the list is given in VISUM format
-	the list describes the spatial course of the line
-	each line route item is characterized by: line name, line route name, direction code, index of the stop, stop (point) number, accumulated length 

## vehjourney
-	the list is given in VISUM format
-	the list summerizes the skims of each vehicle journey 
-	each vehicle journey is characterized by: number of the journey, line name, line route name, direction code, departure time (at first stop), arrival time (at last stop), first stop (point) number, last stop (point) number, sum of the service kilometer

## vehjourneyitem
-	the list is given in VISUM format
-	the list describes the spatial and temporal course of the line
-	each vehicle journey item is characterized by: number of the journey, index of the item, line name, line route name, direction code, stop (point) number of last the last stop,  stop (point) number of last the next stop, arrival time at the stop, departure time the stop, total capacity (seat and standing capacity) of the serving vehicle
-	assignment results for each vehicle journey item is characterized by: boarding passengers, through passengers (remain in the vehicle), alightning passengers, volume

## image
-	line concept and frequency: The line concept is illustrated by the different line colours and the line name at the end of each line. The frequency per hour of the line is listed after the line name in parentheses.
-	link saturation: The link colour represents the saturation. The color bar indicates the saturation on link level. Each link provides the information of the link volume (sum over all lines) and the link capacity (number of public transport trips multiplied by the vehicle capacity).
-	max. vehicle journey saturation: The link colour represents the saturation. The color bar indicates the saturation level on the most loaded vehicle journey. Each link provides the information of the most loaded vehicle journey and the vehicle capacity.