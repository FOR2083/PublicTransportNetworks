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

The current data sets are a result of the research project "[FOR 2083: Integrated Planning For Public Transportation](https://for2083.math.uni-goettingen.de/en/project)" funded by the German Research Association DFG. Data sets are for academic research purposes only. Users are fully responsible for any results or conclusions obtained by using these data sets. Users must indicate the source of any dataset they are using in any publication that relies 
on any of the datasets provided in this web site.  The Research Group FOR 2083 is not responsible for the content of the data sets. Agencies, organizations, institutions and individuals acknowledged in this web site for their contribution to the datasets are not responsible for the content or the correctness of the datasets.

# Summary of Networks

| Network                                            | Zones | Links  | Nodes  | Stops  |
| ---                                                | ---   | ---    | ---    | ---    |
| Grid 5x5                                           |    25 |     80 |     25 |     25 |
| Grid 21x21                                         |   100 |   1680 |    441 |    341 |
| Ring 8x11                                          |   161 |    640 |    161 |    161 |
| Ring 16x22                                         |   672 |   6720 |   2689 |    673 |
| SiouxFalls                                         |    24 |     76 |     24 |     74 |
| Erding											                       |    52 |    146 |     52 |     52 |
| Stuttgart                                          |   588 |   1436 |    577 |    577 |

# Formats
The  data is provided in the following formats
  - text-format [LimTim](https://lintim.math.uni-goettingen.de/index.php?go=main.php&lang=en)
  - text-format [VISUM](http://vision-traffic.ptvgroup.com/en-us/products/ptv-visum/)
  - spreadsheet-format (.xls)
  - binary-format [VISUM](http://vision-traffic.ptvgroup.com/en-us/products/ptv-visum/)
  

# Other Related Projects
- [LinTim](https://lintim.net/)
- [Transportation Networks](https://github.com/bstabler/TransportationNetworks)
