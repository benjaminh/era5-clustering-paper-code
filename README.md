Extreme-event clustering from ERA5 metocean hindcasts (1940-2023) along northwestern Atlantic coast
=====

Jupyter notebooks and dataset to be used for results reproductibility of the scientific paper "AExtreme-event clustering from ERA5 metocean hindcasts (1940-2023) along northwestern Atlantic coast" by Hervy et al.

## Description

This project includes:
- Notebook for preprocessing NetCDF data: loads NetCDF files as pandas Dataframes, and create the set of timeseries to be clustered. Also save data as numpy pickles.
- Notebooks for clustering: loads previous numpy data, and apply KMeans clustering using DTW (resp. feature extraction w/ AutoEncoder architecture)
- Data: raw data as NetCDF files from Copernicus CDS (including additional computed variables for wind), and numpy preprocessed data. 

## Howto

The notebooks can be executed using Anaconda or Miniconda. A list of prerequisites is provided as `environment.yml`, and can be used as follows:
1. Make sure you have `conda` package manager available on your machine, either with Anaconda or Miniconda
2. Create a virtual environment using `environment.yml`: `conda env create -f environment.yml`
3. Activate the environment: `conda activate myenv`
4. Load Jupyter-lab: `jupyter-lab`

## Licence

1. **Python code / Jupyter notebooks**  
   [MIT License](LICENSE-code).

2. **Processed data from ERA5 (ECMWF)**  
   Under CC BY 4.0 – see [LICENSE-data-ECMWF](LICENSE-data-ECMWF).  
   Please cite:
   > Hersbach, H. et al. (2020). ERA5 hourly data on single levels from 1979 to present.  
   > Copernicus Climate Change Service (C3S) Climate Data Store (CDS).  
   > DOI:10.24381/cds.adbb2d47

3. **Results (images, binaries)**  
   [CC-BY 4.0](LICENSE-results)


