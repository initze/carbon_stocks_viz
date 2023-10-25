# carbon_stocks_viz
Visualization of global/permafrost soil carbon stocks

Create a figure to show carbon stocks per latitude + land area and permafrost coverage
## Workflow
### Preprocessing
#### GEE (rester input)
1. Create fishnet (geemap)
* 0.1° Longitude, 1° latitude (-180:180 Lon, -90:90 Lat)
2. Merge fishnet to 1° lat strips
3. use soilgrids soc and bdod to calculate SOC stocks per density in GEE
4. pull sum of carbon stocks per latitude with geemap
5. save to csv

#### Local data (vector input)
1. Create fishnet (geemap)
* 0.1° Longitude, 1° latitude (-180:180 Lon, -90:90 Lat)
2. Merge fishnet to 1° lat strips
3. intersect strips with vector layers (Countries for land area, Brown IPA PF map for permafrost)
4. calculate areas using IAEA projection 

## Results
Version 08
![soil_carbon_v08](https://github.com/initze/carbon_stocks_viz/assets/4864803/e477128a-7095-4299-b5ac-7334e0a82ee5)
