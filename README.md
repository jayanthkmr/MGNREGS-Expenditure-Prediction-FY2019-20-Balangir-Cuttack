# MGNREGS-Expenditure-Prediction-2019-2020
**Aproach 1** is the aggregation of preditions at block level to calculate the AC level expenditure. It was the approach that worked for Balangir district as there wasn't any overlaps in block boundaries over AC, however it wasn't the case for Cuttack or in general for any other district. Also, the boundry for Census block is mostly different from revenue blocks.

**Aproach Final** is the aggregation of preditions at village level to calculate the AC level expenditure. 

The GeoJson for village level boundries were extracted from [here](https://github.com/datameet/indian_village_boundaries)

The shapefile for AC and District boundries were extracted from [here](https://github.com/datameet/maps/tree/master/assembly-constituencies)
