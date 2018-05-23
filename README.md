# Public Transport Networks
Public Transport Networks is a networks repository for public transport research. It provides networks as test instances for the following types of problems:
  - Public transport network design problem (NDP)
  - Public transport vehicle and crew scheduling
  - Public transport networks with disturbances
  - Public transport assignment
  - Handling of ridesharing trips

# How the Data is Organized

Each individual network and related files is stored in a separate folder. Each folder contains the following subfolders:
  - Input: provides data describing the transport supply (nodes, stops, links, running times)  and data describing the travel demand (traffic zones, trips between traffic zones)
  - Solution_NDP_Summary: Overview of all solutions for the Network Design Problem
  -	Solution_NDP_Name: Description of a particular solution for the Network Design Problem 
  
# License 

The current data sets are a result of the research project "FOR 2083: Integrated Planning For Public Transportation" funded by the German Research Association DFG. Data sets are for academic research purposes only.  Users are are fully responsible for any results or conclusions obtained by using these data sets. Users must indicate the source of any dataset they are using in any publication that relies 
on any of the datasets provided in this web site.  The Research Group FOR 2083 is not responsible for the content of the data sets. Agencies, organizations, institutions and individuals acknowledged in this web site for their contribution to the datasets are not responsible for the content or the correctness of the datasets.

# Summary of Networks

| Network                                            | Zones | Links  | Nodes  |
| ---                                                | ---   | ---    | ---    |
| Grid                                               |    25 |     80 |     25 |
| Ring                                               |   161 |    640 |    161 |
| SiouxFalls                                         |    24 |     76 |     24 |
| Stuttgart                                          |    NN |     NN |     NN |

# Formats
The  data is provided in text-format, as spreadsheet and as binary VISUM versionfile. 


## VISUM Text Format 
The VISUM text format is CSV text files, with contains the network and demand data in tabular form.
each row terminated by a semicolon.  The files have the following format:


NET OBJECT	VISUM ATTRIBUTE	DESCRIPTION	UNIT	DATATYPE
NODE	NO	index	[-]	[integer]
NODE	CODE	description	[-]	[string]
NODE	NAME	description	[-]	[string]
NODE	XCOORD	x-coordinate	[-]	[float]
NODE	YCOORD	y-coordinate	[-]	[float]
LINK	NO	index	[-]	[integer]
LINK	FROMNODENO	from node number	[-]	[integer]
LINK	TONODENO	to node number	[-]	[integer]
LINK	LENGTH	length of the link	[km]	[float]
LINK	V0_PRTSYS(P)	speed permitted per private transport system(P=car) in the unloaded state (free flow speed).	[km/h]	[float]
LINK	T_PUTSYS(B)	run time by public transport system(B=bus).	[second]	[float]
LINK	Belastung_Std_ÖV	"volume PuT in [number of persons] (morning peak hour 07:00-08:00)
matrices for the entire day are available.
the loads describe the link volume after the PuT supply has been implemented and load have been assigned to the network. Assignment without capacity restriction."	[-]	[float]
LINK	Kapazität_Std_ÖV	link capacity for PuT systems. Vehicles runs x vehicle capacity.	[-]	[float]
LINK	Auslastung_Std_ÖV	Saturation = Belastung_Std_ÖV / Kapazität_Std_ÖV	[-]	[float]
LINK	Belastung_Std_ÖV	"volume PuT in [number of persons] (morning peak hour 07:00-08:00)
matrices for the entire day are available.
the loads describe the link volume after the PuT supply has been implemented and load have been assigned to the network. Assignment with capacity restriction."	[-]	[float]
LINK	Kapazität_Std_ÖV	link capacity for PuT systems. Vehicles runs x vehicle capacity.	[-]	[float]
LINK	Auslastung_Std_ÖV	Saturation = Belastung_Std_ÖV / Kapazität_Std_ÖV	[-]	[float]
ZONE	NO	index	[-]	[integer]
ZONE	CODE	description	[-]	[string]
ZONE	NAME	description	[-]	[string]
ZONE	XCOORD	x-coordinate	[-]	[float]
ZONE	YCOORD	y-coordinate	[-]	[float]
STOP	NO	index	[-]	[integer]
STOP	CODE	description	[-]	[string]
STOP	NAME	description	[-]	[string]
STOP	XCOORD	x-coordinate	[-]	[float]
STOP	YCOORD	y-coordinate	[-]	[float]
