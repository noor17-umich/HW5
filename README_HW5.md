
# HW5 - Data Visualization and GeoJSON Mapping

This repository contains the work for **HW5**: Data Visualization using R and GeoJSON mapping using ArcGIS and JavaScript.

## Task 1: Data Visualization in R
In this task, we visualized US states and wind turbine locations using the following steps:

1. **Load Data**: 
   - We used the `map_data("state")` function from the `mapdata` library to load geographic information for US states.
   - Filtered out the coordinates for California and stored it in a new dataframe called `california`.

2. **Wind Turbine Data**:
   - Loaded the `wind_turbines.rda` data from the `DATA` folder and filtered the turbines located in California.
   - Created a new dataframe called `wind_ca`.

3. **Visualization**:
   - Used `ggplot()` and `geom_polygon()` to create the map of California.
   - Added wind turbine locations using `geom_point()`.

4. **R Markdown**:
   - An R Markdown file (`HW5.Rmd`) was created to generate the HTML output with the code and map.

## Task 2: Using ArcGIS for GeoJSON Visualization
This task involved visualizing election data on ArcGIS using the `2016elections.geojson` file. The following steps were performed:

1. **Import GeoJSON**:
   - Imported the `2016elections.geojson` file into ArcGIS.

2. **Set Basemap**:
   - Used "Add Charted Territory" as the basemap.

3. **Election Layer**:
   - Added a `2016Election` layer to the map and colored states based on the winner (Trump in red, Clinton in blue).

4. **Web App**:
   - Created a web app to display the map and election results.

5. **Link Submission**:
   - A link to the ArcGIS web app was submitted for review.

## Task 3: Modifying the Choropleth Map in JavaScript
In this task, the **ChoroplethUSMap.html** file was modified to display election results by adjusting JavaScript functions.

1. **Modified JavaScript**:
   - Replaced the source URL in the JavaScript code to point to the `2016elections.js` file.
   - Updated the `getColor()` function to color the states based on the winner (Trump = red, Clinton = blue).

2. **Uploaded HTML**:
   - The modified `ChoroplethUSMap.html` file was uploaded to this repository.

## How to Run

To run the project and view the results, follow these steps:

1. **For Task 1**:
   - Open the `HW5.Rmd` file in RStudio.
   - Click **Knit** to generate the `HW5.html` output.

2. **For Task 2**:
   - Open the ArcGIS web app URL to view the election map.

3. **For Task 3**:
   - Open the `ChoroplethUSMap.html` file in a browser to see the modified choropleth map with election results.

## Files in This Repository

- `HW5.Rmd` - R Markdown file for Task 1.
- `HW5.html` - Generated HTML from the R Markdown file.
- `ChoroplethUSMap.html` - Modified choropleth map HTML file for Task 3.
- `2016elections.geojson` - GeoJSON file used for Task 2.
- `wind_turbines.rda` - Wind turbine data used in Task 1.

## License

This repository is licensed under the MIT License.
