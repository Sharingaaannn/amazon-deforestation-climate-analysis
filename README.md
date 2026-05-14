# 🌳 Amazon Deforestation & Local Climate Change
## Temporal and Spatial Analysis of Temperature Responses in Porto Velho, Brazil (2017–2025)

---

## 📌 Overview

This project investigates how deforestation in Porto Velho, Rondônia, 
Brazil drives local temperature change over time and space. Using 
satellite-based deforestation data and ERA5-Land reanalysis climate 
records, the study quantifies both the lagged warming effects of forest 
loss and the spatial clustering of those impacts across the landscape.

---

## 🔍 Key Findings

- 🌡️ Deforestation causes maximum temperature increases of 1–3°C, 
  with the strongest effects emerging 2–3 years after clearing
- 📈 ARDL models significantly outperformed OLS regression 
  (adjusted R² up to 0.89 vs 0.06)
- 🗺️ Warming effects are spatially clustered along agricultural 
  frontier zones in southern Porto Velho
- ⚠️ Maximum temperatures showed the highest sensitivity to 
  deforestation — increasing heat extremes pose the greatest 
  climate risk

---

## 🛠️ Tools & Methods

| Category | Tools Used |
|---|---|
| Languages | Python |
| Climate Data | ERA5-Land via Google Earth Engine |
| Geospatial | GeoPandas, Rasterio, Folium |
| Time-Series | ARDL Models, OLS Regression (Statsmodels) |
| Spatial Stats | Global Moran's I, LISA Hotspot Analysis (PySAL) |
| Visualisation | Matplotlib, Plotly, Folium |

---

## 📂 Repository Structure

- notebooks/ — Full analysis notebook
  - amazon_deforestation_analysis.ipynb
- data/ — Raw and processed datasets
  - deforestation/ — Monthly deforestation polygons
  - climate/ — ERA5-Land temperature data
- outputs/ — Maps, charts and results
  - figures/
  - maps/

---

## 📊 Methodology

### 1 Temporal Analysis
- Ordinary Least Squares (OLS) regression as baseline
- Autoregressive Distributed Lag (ARDL) models with 
  12, 24 and 36-month deforestation lags
- Separate models for mean, maximum and minimum temperature

### 2 Spatial Analysis
- Per-cell regression to map warming sensitivity across landscape
- Global Moran's I to test for spatial autocorrelation
- LISA (Local Indicators of Spatial Association) to identify 
  hotspots and coldspots
- Interactive Folium maps for visualisation

---

## 🌍 Data Sources

- Deforestation data: INPE (Brazilian National Institute 
  for Space Research) via official Brazilian monitoring systems
- Climate data: ERA5-Land reanalysis — European Centre 
  for Medium-Range Weather Forecasts (ECMWF) via Google Earth Engine
- Study period: January 2017 to May 2025
- Study area: Porto Velho municipality, Rondônia, Brazil

---

## 📋 Policy Implications

- Short periods of deforestation can lock in multi-year warming
- Targeted protection of frontier hotspot zones could 
  deliver disproportionate climate benefits
- Evidence supports enforcement of Brazil's Forest Code and 
  international commitments under the Paris Agreement

---

## 👤 Author

Asim Fulzele
MSc Environmental Data Science & Analytics

- LinkedIn: (https://www.linkedin.com/in/asim-fulzele-62a8b419a/ )
- Email: asimfulzele16@gmail.com
