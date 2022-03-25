# README

This repo includes supporting material for Qiu et al., Science Advances, 2022 "Impacts of wind power on air quality, premature mortality and environmental justice in the US". 

## Regression results: 
*EGU_regression_scenario_results.xlsx*  
It includes regression result for each EGU in our sample (1264 EGUs in total). 

## Simulation results
### GEOS-Chem simulation
*GC_daily_pm25_o3_scenarios.nc*  
It contains surface level annual mean PM2.5 and MDA8 O3 concentration under different emission scenarios. We include four scenarios in total:
- baseline scenario: air quality **without** the amount of wind power associated with 2014 RPS targets 
- expost scenario:  air quality with the wind power associated with 2014 RPS targets under the current dispatch decisions
- health damage minimizing scenario: air quality with the wind power associated with 2014 RPS targets under a hypothetical dispatch scenario that minimizes the health damage
- CO2 minimizing scenario: air quality with the wind power associated with 2014 RPS targets under a hypothetical dispatch scenario that minimizes the CO2 emissions

Therefore, to calculate the air quality impacts of wind power under different dispatch decision:  
current (ex post) = ex post - baseline.  
health damage minimizing =  health damage minimizing - baseline.  
CO2 minimizing scenario = CO2 minimizing - baseline.  

### InMAP simulations
*InMAP/xx.shp*   
The shapefiles contain annual mean PM2.5 concentration simulated with InMAP under different emission scenarios.  
baseline.shp: baseline scenario  
ex post.shp: ex post scenario  
health_damage_minimizing.shp: health damage minimizing scenario  
co2_minimizing.shp: CO2 minimizing scenario

Descriptions of the four scenarios are the same as above for GEOS-Chem.

## County-level air quality change for different demographic groups
*county_pm_o3_changes_by_groups_GEOS_CHEM.xlsx*  
This file contains changes in county-level simulated PM2.5 and O3 concentrations due to wind power under different scenarios. It also includes the total population at the county level and population for each subgroup. This data can be used to calculate the distributional effects of air quality benefits across different population groups.


