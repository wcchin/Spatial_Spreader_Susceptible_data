# The preprocessing data

This directory include the data after the preprocessing and networks prepared for the analysis. 



1. scaled_bus_OD: the OD flow is scaled down using the bus stop in-and-out data, in each month, 
2. merge_bus_and_train: the merged data of the bus and train OD flow according to their location subzone, i.e. 303 to 303 OD, in each month, 
3. weekday_network_main.net: the main network file for weekday analysis, 
4. weekend_network_main.net: the main network file for weekend analysis, 
5. weekday_network_adjusted_for_mapequation: the weekday network with the flow adjusted (inversed distance weighting, IDW) using the equation as described in the paper (and following), 
6. weekend_network_adjusted_for_mapequation: same as above, for weekends. 



The IDW equation: 
$$
F'(o,d) = \frac{F(o,d)}{\text{distance}(o,d)}
$$
where, $F(o,d)$ is the raw flow between subzones $o$ and $d$, $\text{distance}(o,d)$ is the straight distance between the centroid of the two subzones, and $F'(o,d)$ is the adjusted flow. 



The scale-down process is calculated using the total tap-in/out and the total flow in OD as the scale factor for each month.