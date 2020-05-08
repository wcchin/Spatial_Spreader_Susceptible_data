# The calculation results

This directory contains the intermediate and final calculation results. 

- 1_node_stat_normalized.csv: The node-based in/out degree in weekdays and weekends, normalized to unit interval (0-1), 
- zone analysis:
  - 2a_weekday_zones.csv: the mapequation results of weekdays, 
  - 2b_weekend_zones.csv: the mapequation results of weekends, 
  - 2c_zone_entropy.csv: the in/out neighbor zone-entropy, 
- coreness analysis: 
  - 3a_coreness_k_shell_wlvl.csv: the incoming/outgoing $k$-shell decomposition results and core/periphery level, 
  - 3b_coreness_entropy.csv: the in/out coreness-entropy, 
- 4_SPI_and_SUI.csv: the weekdays and weekends spreader/susceptible index, 
- 5_SSP_and_SSS.csv: the spatial super spreaders and spatial super susceptibles. 



## About the columns 

2c_zone_entropy.csv: 

1. ind: index, 
2. node: subzone name (for join), 
3. level_1_weekday: weekday community ID, 
4. level_1_weekend: weekend community ID, 
5. weekday_com_ent_in: the community entropy of incoming neighhors, weighted by the incoming flows, 
6. weekday_com_ent_out: same as above, but using outgoing neighbors and flows, 
7. weekend_com_ent_in: same as 5, for weekends, 
8. weekend_com_ent_out: same as 6, for weekends. 



3b_coreness_entropy.csv: 

1. ind: index, 
2. node: subzone name (for join), 
3. weekday_in_core: weekday incoming $k$-shell value, 
4. weekday_out_core: weekday outgoing $k$-shell value, 
5. weekend_in_core: same as 3, for weekends, 
6. weekend_out_core: same as 4, for weekends, 
7. weekday_in_core_lvl: group the subzones into core/periphery using median value as cutoff, for weekday incoming $k$-shell value (the levels: $1$ means core, $0$ means periphery), 
8. weekday_out_core_lvl: same as 7, for weekday outgoing $k$-shell value,
9. weekend_in_core_lvl: same as 7, for weekends, 
10. weekend_out_core_lvl: same as 8, for weekends, 
11. weekday_ksc_ent_in: the weekday incoming coreness-entropy,  
12. weekday_ksc_ent_out: the weekday outgoing coreness-entropy,  
13. weekend_ksc_ent_in: same as 11, for weekends, 
14. weekend_ksc_ent_out: same as 12, for weekends. 



