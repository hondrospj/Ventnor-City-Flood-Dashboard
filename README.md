# Roads at Risk

Static GitHub Pages app for drawing cross sections through a clipped 5 ft Ventnor City DEM.

Cross sections can be saved as a multi-line map collection. The active line drives the elevation and flood-history charts, while exports can include every saved section as CSV, an ESRI Shapefile ZIP, or a combined CSV + Shapefile ZIP.

DEM source: USGS 3DEP Bare Earth DEM Dynamic ImageServer, clipped to the Ventnor City boundary and resampled to 1.524 m / 5 ft pixels.

Flood-dashboard context: Inside Thorofare at Atlantic City observations, Ventnor City thresholds, dated observed daily peaks, top tide events, high tide count, and trend summary are stored in `flood_stats.json`. The closest PETSS station is `est4836` / `8534836`.

Main files:

- `index.html` - web app
- `ventnor_city_dem_5ft_cog.tif` - elevation COG, meters
- `ventnor_city_hillshade.png` - map hillshade preview
- `ventnor_city_boundary.geojson` - clip boundary
- `dem_metadata.json` - data provenance and raster bounds
- `flood_stats.json` - flood-dashboard thresholds, dated archive peaks, and trend statistics used by dot-click flood charts
