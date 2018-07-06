# Grid 5x5 Instance

## Description
A grid network with 5 rows and 5 columns.

![grid_network]()

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

![02_grid_demand_en 2](https://user-images.githubusercontent.com/30687001/42214595-33c43990-7ebc-11e8-9bcd-4712eb89d246.jpg)

Attention: only the first 100 greatest values for odpairs are displayed.
![02_grid_relocation_en 2](https://user-images.githubusercontent.com/30687001/42366281-16008ffc-8101-11e8-8692-af2c0e6161b6.jpg)

## Vehicle and Operating Cost Data
One vehicle type with a capacity of 70 places is available. The costs for one vehicle including the driver amount to 50 $/h and 1.50 $/km. Different to interlining trips, pull-out and pull-in trips from and to the depot are not considered. There are no minimum layover times at the terminals.

| Vehicle           | Value  | Unit     | 
| ---               | ---    |---       |
| Capacity          |     70 |  [Places]|
| Operating Cost/h  |  50.00 |[Monetary]|
| Operating Cost/km |   1.50 |[Monetary]|

## Transfer Time
Every transfer requires a minimum transfer time of 3 minutes.

| Transfer           | Value  | Unit     | 
| ---                | ---    |---       |
| Min. transfer time |      3 |[min]     |

## Perceived Journey Time
Evaluating the service quality considers in-vehicle time IVT, transfer wait time TWT and number of transfers NoT. Every transfer is weighted with a time penalty of 5 minutes. Access and egress times are not included. For the route choice in the assignment and for evaluating the service quality a perceived journey time is computed

PJT = 1.0 * IVT + 1.0 * TWT + 5.0 * NoT. 

| Factor            | Value  | Unit         | 
| ---               | ---    |---           |
| in-vehicle time   |    1.0 |  [-]         |
| transfer wait time|    1.0 |  [-]         |
| transfer          |    5.0 |[min/transfer]|
