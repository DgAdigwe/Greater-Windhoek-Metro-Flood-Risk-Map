Greater Windhoek Flood Risk Map
This project presents a flood risk map of Greater Windhoek, Namibia, developed using openly available geospatial datasets and processed in QGIS. The aim is to provide a general overview of potential flood-prone areas by integrating hydrological, climatic, topographic, and land cover data.

Data Sources
The following datasets were used:
	SoilGrids (ISRIC) – Soil properties, including clay and sand fractions for infiltration analysis.
	WorldClim – Historical precipitation and climate data for rainfall distribution.
	SRTM 30m (NASA/USGS) – Digital Elevation Model (DEM) for terrain slope, elevation, and hydrological modelling.
	ESA Land Cover (CCI / Copernicus) – Land use and land cover classification for vegetation and building cover.

Methodology
Data Preprocessing:
	Reprojected all datasets to a common coordinate system (UTM Zone 33S).
	Clipped data to the Greater Windhoek boundary.
	Resampled all data to 30 pixels

Criteria Development:
Elevation & Slope (SRTM 30): Low-lying and gentle slope areas were considered more flood-prone.
Soil Properties (SoilGrids): Clay-rich soils were assigned a higher flood risk due to poor infiltration.
Precipitation (WorldClim): Areas with higher rainfall values were considered higher risk.
Land Cover (ESA): Urban areas and bare land were weighted higher due to reduced infiltration.
Drainage Density(SRTM 30): the higher the drainage density concentration, the higher the flood risk.
Proximity to Streams(SRTM 30): Closer to a stream, the higher the risk of flooding.

Flood Risk Index Calculation:
Normalised each factor to a common scale.
Applied weighted overlay analysis to combine layers into a Flood Risk Index (FRI).

Risk Zonation:
Final flood risk map categorised into very low, Low, Moderate, High, and Very High Risk zones.

Disclaimer
This flood risk map is a general representation based on publicly available datasets and simplified assumptions. While every effort was made to ensure accuracy, the results do not replace detailed hydrological or engineering studies. Local-scale flood risk assessments should be carried out for planning, design, or disaster management purposes.

Applications
	Preliminary flood hazard awareness.
	Support for urban planning and risk reduction strategies.
	Educational and research purposes.

License
This project is open-source and available under the MIT License.

Author
Dimnaka Adigwe
LinkedIn: http://www.linkedin.com/in/dimnaka-adigwe-164b10168 
Email: adigwenaka@gmail.com
