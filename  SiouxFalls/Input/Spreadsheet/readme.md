# Spreadsheet Input Format
The input spreadsheet contains the following tables to describe the network supply:
-	summary
-	attribute
-	node
- 	link
-	zone
-	stop
-	odpair	
-	image

## summary
-	the sheet lists typical characteristics of the network for input values
-	two pictures are embedded to show the network instrastruktur and the demand situation  

## attribute
-	the list describes the available attributes for each network object
-	each attribute is characterized by networkobject name, VISUM attribute name, description, unit and datatype

## node
-	the list is given in VISUM format to provide a reimport to VISUM
-	each node is characterized by number, code, name, xcoord, ycoord

## link
-	the list is given in VISUM format to provide a reimport to VISUM
-	each link is haracterized by number, from node number, to noden number, length, maximum privat transport speed limit, public transport travel time

## zone
-	the list is given in VISUM format to provide a reimport to VISUM
-	each zone is characterized by number, code, name, xcoord, ycoord

## stop
-	the list is given in VISUM format to provide a reimport to VISUM
-	each stop is characterized by number, code, name, xcoord, ycoord

## odpair
-	the list is given in VISUM format to provide a reimport to VISUM
-	each odpair is characterized by from node number, to node number, sum of the total demand, sum of privat transport demand, sum of public transport, sum of public transport during peak hour

## image
-	network situation with link length travel time
-	travel demand situation for each zone with originating and terminating traffic
-	travel demand situation for relocating demand