# Shelter_ML

# Overview
Prediction of Forest fire, weather, and earthquake on the Province of North Sumatera. Dataset used is from BMKG, KLHK, and Geonames Dataset.

# Process
1. Collect 5 years climate and earthquake data from BMKG (1st Jan 2016- 31st Dec 2020)
2. Collect 5 years forest fire data from SiPongi KLHK (1st Jan 2016- 31st Dec 2020)
3. Collect GeoNames Dataset and filter it using polygons, so only North Sumatra Remains.
4. Do a time-series seasonal forecasting using SARIMAX from weather and earthquake data for one year ahead (1st Jan 2021-31st Dec 2021)
5. Use haversine formula to find nearest town from the forecasted earthquake
6. Use haversine formula to determine the distance between detected forest fires/hotspot and nearest town, then merge it with forest fire data, and use it as human variables
7. Merge weather data with forest fire data based on date, and use it as weather variables
8. Do a Regression modeling on the forest fire dataset, and save the model
9. Use the weather forecast we make earlier to predict possible forest fires
10. Hand-over the results to cloud computing as excel and KML





# Mobile
Documentation : https://github.com/alfalifr/Shelter_Mobile

# Cloud Computing
Documentaion : https://github.com/alfalifr/Shelter_Cloud