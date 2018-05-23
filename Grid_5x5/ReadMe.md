# Grid 5x5 Instance

## Description
A grid network with 5 rows and 5 columns.

## Supply Data
| Network       | Value  | Unit |
| ---           | ---    |---   |
| Zones         |     25 | [-]  |    
| Nodes/stops   |     25 | [-]  |   
| Links         |     80 | [-]  |

## Demand Data
| Demand       | Value  | Unit       | 
| ---          | ---    |---         |
| OD-pairs     |    600 | [-]        |
| Trips        |   2531 | [Trips/h]  |

## Transfer time
Every transfer requires a minimum transfer time of 3 minutes.
| Transfer           | Value  | Unit     | 
| ---                | ---    |---       |
| Min. transfer time |      3 |[min]     |


## Perceived Journey Time
Evaluating the service quality considers in-vehicle time, transfer wait time and number of transfers. Every transfer is weighted with a time penalty of 5 minutes and requires a minimum transfer time of 3 minutes. Access and egress times are not included, as the stop locations are given and stop location choice is not taken into account.

| Factor            | Value  | Unit         | 
| ---               | ---    |---           |
| in-vehicle time   |    1.0 |  [-]         |
| transfer wait time|    1.0 |  [-]         |
| transfer          |    5.0 |[min/transfer]|
