The GeoJson for village level boundries were extracted from [here](https://github.com/datameet/indian_village_boundaries)

The shafefile for AC and District boundries were extracted from [here](https://github.com/datameet/maps/tree/master/assembly-constituencies)

In this approach, village data for each assembly constituency was derived by putting the condition to the village boundary file. The villages whose centroid fell under the AC boundry was taken into consideration. The data for these selected villages were extracted fron census population enumeration data and used to predict the expenditure for the ACs in Balangir and Cuttack.

Refer to MGNREGS_expenditure_prediction _for _Cuttack_Balangir.ipynb for more details on the methodology. 
Go to file
