# Change Detection with GEE and SAR data for Sviatohirsk, Ukraine

## Pre-requisites:
1. Google Earth Engine account
1. Miniconda or Anaconda environment with >= Python 3.7
1. VSCode and Jupyter Notebook
1. Git installed and GitHub account

## Preparation steps:
1. Clone the repository
1. Create a new conda environment
1. Install the required packages
1. Authenticate with GEE
1. Run the Jupyter Notebook

## Data sources:
1. OpenStreetMap
1. Microsoft Building Footprints
1. Sentinel-1 SAR data from GEE (VV and VH polarizations)

## Stages of the project:
1. Download buildings from OSM & Microsoft Building Footprints
1. Upload datasets to GEE
1. Process SAR data and create change detection maps
1. Overlay change detection maps with building footprints
1. Export footprint polygons with change detection information

## Results:
1. Change detection maps
1. Building footprints with change detection information
