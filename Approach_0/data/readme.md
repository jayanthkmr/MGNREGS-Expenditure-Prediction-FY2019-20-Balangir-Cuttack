# Approach 0: Geospatial Prediction at AC Level

## Overview
This approach predicts the MGNREGS expenditure using geospatial data (Area, Perimeter, Latitude, and Longitude) extracted from AC level boundaries.

## Data Requirements
- Geospatial data from QGIS detailing the AC level boundaries.
- CSV or GeoJSON files containing the fields: Area, Perimeter, Latitude, and Longitude of centroid.

## Running the Model
To execute the prediction model:
```bash
jupyter Notebook
```

## Expected Output
- Predictions of expenditure at the AC level as output files in CSV format.
- Visualizations of the predicted expenditures if applicable.
