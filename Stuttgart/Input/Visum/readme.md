# VISUM Format
The input contains the following files to describe the network supply:
-	Demand.mtx: text file with demand data
-	Fixed_Lines.net: regional rail supply
-	Infrastructure.net: text file with supply data
-	Versionfile.ver: binary demand and supply data in VISUM Format 

An additional explanation of the files is given below for each input file.

## Demand.mtx
The Demand.mtx file provides information of the demand on origin-destination level in the VISUM specific $O Format. The demand is given as float numbers. 


## Fixed_Lines.net
The Fixed_Lines.net file contains the regional rail supply in VISUM net file format. It is readable with a text editor. The net file can be directly imported to a VISUM instance. It includes the following net objects in a descending order: 
-	VISION: main header of net file license information and date of export
-	Table: Lines
-	Table: Line routes
-	Table: Line route items
-	Table: Time profiles
-	Table: Time profile items
-	Table: Vehicle journeys
-	Table: Vehicle journey items
-	Table: Vehicle journey sections


## Infrastructure.net
The Infrastructure.net file contains the network supply in VISUM net file format. It is readable with a text editor. The net file can be directly imported to a VISUM instance. It includes the following net objects in a descending order: 
-	VISION: main header of net file license information and date of export
-	Table: Version Block
-	Table: Nodes
-	Table: Zones
-	Table: Links
-	Table: Connectors
-	Table: Stops
-	Table: Stop areas
-	Table: Stop points


## Versionfile.ver
-	The Versionfile.ver file contains the complete network in a binary-format. The versionfile can be opened with PTV VISUM 20 or later. 