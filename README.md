# EMT Madrid Demand Analysis 🚌

An interactive Tableau dashboard analyzing demand patterns in Madrid's EMT bus network using open data and Python.

This project combines temporal and spatial analysis to explore ridership trends, identify usage patterns, and highlight the most heavily used bus lines between 2019 and 2025.

## Project Objectives

- Analyze demand evolution between 2019 and 2025.
- Compare ridership on weekdays and non-working days.
- Identify weekly and seasonal demand patterns.
- Explore the spatial coverage of the bus network.
- Detect the most frequently used bus lines.

## Technologies Used

- Python
- Pandas
- PyProj
- Tableau
- Madrid Open Data Portal

## Data Sources

Datasets obtained from the Madrid Open Data Portal:

- `stopsemt.csv` - https://datos.madrid.es/dataset/900023-0-emt-paradas-autobus
- `demandalinea.csv` - https://datos.madrid.es/dataset/900028-0-emt-demanda-autobus

## Data Preparation

The main preprocessing tasks included:

- Removing invalid records.
- Handling missing values.
- Filtering duplicate routes using the direction field.
- Converting coordinates from EPSG:25830 to EPSG:4326.
- Creating date-derived features:
  - Year
  - Month
  - Day of Week
  - Working Day / Non-Working Day
- Excluding 2026 records due to incomplete yearly data.
- Relating both datasets through the `Linea` field.

## Dashboard Overview

The dashboard is divided into two main analytical areas.

### Temporal Analysis

- Yearly demand evolution
- Weekly demand patterns
- Monthly seasonality analysis
- Comparison between working and non-working days

### Spatial Analysis

- EMT network coverage
- Top 10 most-used bus lines
- Geographic visualization of routes

## Key Features

- Interactive filters by year, month and day type
- Rich tooltips with additional context
- Cross-filtering between visualizations
- Dynamic highlighting of minimum and maximum values
- Hover interactions between rankings and map visualizations

## Key Findings

- Demand experienced a significant drop in 2020 followed by a gradual recovery.
- Weekdays account for the majority of passengers.
- Clear seasonal patterns can be observed, with lower demand during summer months.
- A relatively small number of routes concentrate a large share of total ridership.
- Network coverage is particularly dense in central areas of Madrid.

## Dashboard Screenshots

### Dashboard Overview

<img width="1708" height="960" alt="dashboardActividad3" src="https://github.com/user-attachments/assets/e3f1bf09-f93f-4ea9-bc8a-20cc123bc23d" />

### Interactive Demo

<img width="800" height="447" alt="ezgif com-video-to-gif-converter" src="https://github.com/user-attachments/assets/d83af65a-2478-4efd-b6d9-fc2aa8a69631" />


## Skills Demonstrated

- Data Cleaning and Transformation
- Geospatial Data Processing
- Exploratory Data Analysis (EDA)
- Data Visualization
- Dashboard Design
- Business Intelligence
- Tableau Development

## Author

**Marta B**

Data & AI Engineer

LinkedIn: https://www.linkedin.com/in/marta-benito-serrano/
