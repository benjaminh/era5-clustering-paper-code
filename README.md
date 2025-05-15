Extreme coastline morphogenic events analysis from clustering of ERA5 timeseries
=====

Jupyter notebooks and dataset to be used for results reproductibility of the scientific paper "Extreme coastline morphogenic events analysis from clustering of ERA5 timeseries" by Hervy et al.

## Description

This project includes:
- Notebook for preprocessing NetCDF data: loads NetCDF files as pandas Dataframes, and create the set of timeseries to be clustered (Chapter 3.). Also save data as numpy pickles.
- Notebooks for clustering (Chapter 4.): loads previous numpy data, and apply KMeans clustering using DTW (resp. feature extraction w/ AutoEncoder architecture)
- Data: raw data as NetCDF files from Copernicus CDS (including additional computed variables for wind), and numpy preprocessed data. 

## Howto

The notebooks can be executed using Anaconda or Miniconda. A list of prerequisites is provided as `environment.yml`, and can be used as follows:
1. Make sure you have `conda` package manager available on your machine, either with Anaconda or Miniconda
2. Create a virtual environment using `environment.yml`: `conda env create -f environment.yml`
3. Activate the environment: `conda activate myenv`
4. Load Jupyter-lab: `jupyter-lab`

