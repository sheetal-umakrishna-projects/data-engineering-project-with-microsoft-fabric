# Earthquake Data Engineering Project with Microsoft Fabric

## Project Overview
This project demonstrates building a **data engineering and analytics pipeline** using **Python, PySpark, and Microsoft Fabric**. It ingests real-time earthquake events data from the [USGS API](https://earthquake.usgs.gov/) and processes it through **Bronze, Silver, and Gold layers** to create **business-ready datasets** for analysis and visualization in **Power BI**.

This project provides hands-on experience in **data cleaning, transformation, and end-to-end data engineering workflows** using Python.

**Technologies Used:** Python, PySpark, Microsoft Fabric (Data Engineering, Data Factory, Power BI)

---

## Project Workflow

The pipeline is structured in **three layers**, following standard data engineering practices:

1. **Bronze Layer – Raw ingestion**  
   Collects earthquake data from the USGS API with minimal transformation, creating a foundational dataset for downstream processing.  

2. **Silver Layer – Data cleaning and transformation**  
   Cleans and transforms the Bronze dataset, consolidating records and preparing the data for analysis.  

3. **Gold Layer – Business-ready datasets**  
   Produces refined datasets optimized for reporting and visualization in **Power BI**.

All layers are implemented in **Python using PySpark**, demonstrating scalable data processing and integration with Microsoft Fabric.

---

## Repository Contents

- **`Worldwide Earthquake Events API - Bronze Layer Processing.ipynb`**  
  Raw ingestion of USGS earthquake data, stored in original format.  

- **`Worldwide Earthquake Events API - Silver Layer Processing.ipynb`**  
  Cleans and transforms the Bronze dataset into an analytical-ready format.  

- **`Worldwide Earthquake Events API - Gold Layer Processing.ipynb`**  
  Generates business-ready datasets for analysis and visualization.

---

## Data Attribute Definitions

| Attribute | Description |
|-----------|-------------|
| `id` | Unique record identifier (string) |
| `latitude` | Latitude of the earthquake event (double) |
| `longitude` | Longitude of the earthquake event (double) |
| `elevation` | Elevation in meters where the event occurred (double) |
| `title` | Event title or name (string) |
| `place_description` | Location description (string) |
| `sig` | Significance score (bigint) |
| `mag` | Magnitude of the earthquake (double) |
| `magType` | Type of magnitude scale used (string) |
| `time` | Event timestamp (datetime) |
| `updated` | Last update timestamp (datetime) |
