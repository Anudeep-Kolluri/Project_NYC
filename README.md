# NYC Taxi Data Analysis and Visualization Pipeline

## Project Description
This project utilizes **Dagster** and **DuckDB** to create a data pipeline for analyzing and visualizing New York City taxi trip data, specifically focusing on trips in Manhattan. The pipeline integrates geospatial analysis using **GeoPandas** and visualizes the results with **Plotly**. Key tasks include generating statistics on taxi trips by zone in Manhattan and analyzing weekly trip data, with outputs stored as CSV and GeoJSON files.

## Features
1. **Manhattan Taxi Trip Statistics:**
   - Queries taxi trip data from DuckDB to calculate the number of trips in each zone in Manhattan.
   - Uses GeoPandas to transform the zone geometries for geospatial analysis.
   - Saves the resulting data as a GeoJSON file for further visualization.

2. **Manhattan Taxi Trip Map Visualization:**
   - Creates a choropleth map visualizing the number of taxi trips per zone in Manhattan.
   - The map uses Plotly's Mapbox for a detailed and interactive visualization.
   - Outputs the map as an image file.

3. **Weekly Taxi Trip Aggregation:**
   - Aggregates taxi trip data on a weekly basis, summarizing total trips, distance, fare amount, and passenger count.
   - Results are saved as a CSV file for analysis.

## Dependencies
- **Dagster:** Orchestration of the data pipeline assets.
- **DuckDB:** Querying and analyzing taxi trip data.
- **GeoPandas:** Handling geospatial data for taxi zones.
- **Plotly:** Visualizing the data with interactive maps.
- **Pandas:** Data aggregation and processing.

## Outputs
- `manhattan_stats.geojson`: A GeoJSON file containing taxi trip statistics for Manhattan zones.
- `manhattan_map.png`: A choropleth map visualizing the number of trips per zone.
- `trips_by_week.csv`: A CSV file summarizing weekly taxi trip statistics.

This pipeline allows for robust geospatial and temporal analysis of NYC taxi data, providing insights through automated workflows.
