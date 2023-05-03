# Estimating-Global-Horizontal-Irradiance-of-Solar-Photovoltaic-System-from-Satellite-Data

With the spirit of reproducible research, this repository contains all the codes required to produce the results in the manuscript:

Please cite the above paper if you intend to use whole/part of the code. This code is only for academic and research purposes.

# Code Organization

- `model & results.ipynb` Predictive Modelling of the data after gaining insights from EDA.
- `eda & plots.ipynb`Conducted statistical tests, analyzed data distributions, and selected relevant feature spaces to gain a comprehensive understanding of the data.
- `eda & plots - plotly.ipynb`  Utilized Plotly to generate more visually appealing plots and enhance data visualization.
- `download data.ipynb`  To download satellite data from CDS(NOAA)

## Data Files

We're using 2 sources of data in our analysis, 

1. Land Based GHI data is sourced from [Solcast website](https://solcast.com/).

Registering at Solcast will be provide you some free credits. The free credits would be sufficient for successfully recreating this analysis. The request would have the following City Name (Dublin here), Time Period (7 years here) and Parameters (GHI here).
    
2. Satellite Based GHI data is collected from [Climate Data Store (CDS) website](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels?tab=overview) by making API Calls.

For requesting data through API, we have to install CDS Server & Key. Also have to register at CDS & upon aggreeing to their Terms & Conditions we will be provided an api-key to complete the transcation. After completing the whole setup, you can run `download data.ipynb` to obtain the satellite data. Please refer to [Official Wiki](https://cds.climate.copernicus.eu/api-how-to) for more details. 
