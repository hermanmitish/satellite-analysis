## Install additinal libraries and packages

### GDAL 
- GDAL and ogr2ogr is a command line tool that converts one file format to another.

Best just to follow instructions here: https://gdal.org/download.html
Or you can try installing it with conda:
```bash
conda install -c conda-forge gdal
```
Or you can try installing it with brew (MacOS):
```bash
brew install gdal
```

### NVM (Node Version Manager)
- is a version manager for Node.js. With Node.js we can make interactive maps with Mapbox GL JS.

For MacOS:  https://github.com/nvm-sh/nvm
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```

For Windows: https://github.com/coreybutler/nvm-windows/releases


## How to scrape data from Vector Tiles in web maps
- Open the web map in a browser
- Open the developer tools
- Go to the network tab
- Filter by XHR
- Look for requests that end in .pbf
- Right click on the request and copy URL
- Modify the URL to include {z}/{x}/{y}.pbf instead of the specific tile coordinates
- Resulting URL should look like this: https://cdn.kadastr.live/tiles/maps/kadastr/{z}/{x}/{y}.pbf

### With above url, you can add the Vector Tiles layer to QGIS

Or, you can try to scrape it with the 5-admin-zones.ipynb script, just replace the url with the one you copied from the network tab.
You can copy that script and modify it to scrape other layers from the web map.