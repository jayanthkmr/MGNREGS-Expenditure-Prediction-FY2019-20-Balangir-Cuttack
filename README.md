# MGNREGS Expenditure Prediction for FY2019-20

## Project Description
This project aims to predict the expenditure for the Mahatma Gandhi National Rural Employment Guarantee Scheme (MGNREGS) in the districts of Balangir and Cuttack for the fiscal year 2019-20. We utilize geospatial and census data to estimate expenditures at various administrative levels using three distinct approaches.

## Requirements and Installation
- Python 3.8+
- Required Libraries:
  ```
  pip install pandas numpy matplotlib
  ```
- Clone the repository:
  ```
  git clone [repository-url]
  ```

## Usage
To run the prediction models, navigate to the respective approach directory and execute the Python scripts or Jupyter Notebooks:
  ```
  cd Approach_0
  jupyter Notebook
  ```

## Data Sources
The GeoJson for village level boundaries were extracted from [here](https://github.com/datameet/indian_village_boundaries)

The shapefile for AC and District boundaries were extracted from [here](https://github.com/datameet/maps/tree/master/assembly-constituencies)

Block level and village data were extracted from [population enumeration](https://censusindia.gov.in/2011census/population_enumeration.html) data of 2011 census.

- Village level GeoJson boundaries: [Indian Village Boundaries](https://github.com/datameet/indian_village_boundaries)
- AC and District shapefiles: [Assembly Constituencies Maps](https://github.com/datameet/maps/tree/master/assembly-constituencies)
- Census data: [2011 Population Enumeration](https://censusindia.gov.in/2011census/population_enumeration.html)

## Results and Discussion
Each approach is evaluated based on its accuracy and practical applicability. Approach 0 works well under specific conditions, whereas Approach_Final provides a more robust model by aggregating at the village level.

**Aproach_0** has used Area, Perimeter, Latitude and Longitude of the centroid for AC level boundary from QGIS to predict the expenditure across ACs in Balangir and Cuttack. 

**Aproach_1** is the aggregation of predictions at block level to calculate the AC level expenditure. It was the approach that worked for Balangir district as there wasn't any overlaps in block boundaries over AC, however it wasn't the case for Cuttack or in general for any other district. Also, the boundry for Census block is mostly different from revenue blocks.

**Aproach_Final** is the aggregation of predictions at village level to calculate the AC level expenditure. 

## Contributing
We welcome contributions from the community. Please fork the repository, make your changes, and submit a pull request for review.

## License
This project is licensed under the MIT License.

## Contact
For any further queries, please contact jayanthjaiswal15@gmail.com
