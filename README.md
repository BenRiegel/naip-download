# Automated Imagery Downloads

Large GIS and remote sensing projects often incorporate a large number of data files, which must be downloaded from the web and processed. This can be time-consuming and tedius to do individually. This project demonstrates how we can use python to streamline and automate these tasks.

The USGS hosts the National Map website (https://apps.nationalmap.gov/downloader/) at which you can search for data for a particular area of interest. You can create a list of imagery files that intersect the area of interest. The "data.csv" file in the data folder contains a list of NAIP tiles for an area on the coast of Maine. It contains info for 36 tiles. 

In this project, we will use the data to automate the process of downloaded and processing the imagery tiles. In the "download.ipynb" notebook, I walk through the steps of reading the data into a dataframe, extracting the url and file names, downloading the files, and then extracting the bounding geometry from the tiles and saving it to a shapefile. The imagery tiles are saved to the "tiles/img" folder and the resulting shapefile is saved to the "tiles/boundaries" folder. The "environment.yml" file contains a list of all the python packages that the code requires to work.