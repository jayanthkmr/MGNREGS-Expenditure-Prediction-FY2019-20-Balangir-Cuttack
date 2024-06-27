# Approach Final: Village Level Aggregation to AC Level

## Overview
This final approach uses village level data to predict expenditures at the AC level, addressing issues like boundary overlaps found in other approaches.

In this final approach, village data for each assembly constituency was derived by putting the condition to the village boundary file. The villages whose centroid fell under the AC boundry was taken into consideration. The data for these selected villages were extracted fron census population enumeration data and used to predict the expenditure for the ACs in Balangir and Cuttack.

## Data Requirements
- Village level expenditure and demographic data.
- GeoJson for village boundaries.

The GeoJson for village level boundries were extracted from [here](https://github.com/datameet/indian_village_boundaries)

The shapefile for AC and District boundries were extracted from [here](https://github.com/datameet/maps/tree/master/assembly-constituencies)

## Running the Model
```bash
jupyter Notebook
```
Refer to MGNREGS_expenditure_prediction _for _Cuttack_Balangir.ipynb for more details on the methodology. 

## Expected Output
- AC level expenditure predictions based on village data aggregation.
- Visualization of village and AC level data if applicable.


