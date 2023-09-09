# MSc Code 

This repository contains the data download and analysis pipeline designed to enrich andanalyse incident reports provided by WMFS> 

## Data Flow

1. Inital data is queried or request from WMFS.
2. The 'external_data_download.ipynb' notebook enriches this data with additional property and weather details. 
3. The 'analysis.ipynb' notebook takes the enriched data and performs further analsis, modelling and visualisation. 

## Directory Structure

```
data_analysis_pipeline/
├── external_data_download.ipynb # Notebook for downloading/requesting external data via API
├── analysis.ipynb # Notebook for data analysis
├── data/ # Data files (excluded due to sensitive info)
└── README.md # This README file
```



## Notebooks

### `external_data_download.ipynb`

This notebook contains the data analysis process. It uses UPRN (Unique Property Reference Number) information from the incident reports to download or request additional data. The types of data downloaded include:

- Property-specific details
- Weather data at the time of the incident

### `analysis.ipynb`

This notebook performs multiple steps:

1. Extracts semantic information from communications data.
2. Applies predictive models to the structured data.
3. Assesses the validity and reliability of the models.
4. Visualizes the results.

