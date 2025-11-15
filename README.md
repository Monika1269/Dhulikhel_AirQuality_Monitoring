# Dhulikhel_AirQuality_Monitoring
Interactive Weekly Air Quality Monitoring Dashboard for Dhulikhel Using Sentinel-5P on Google Earth Engine

This project is an **interactive air-quality visualization dashboard** designed for **Dhulikhel Municipality**, Nepal.  
It uses **Sentinel-5P TROPOMI** datasets to compute **weekly averages** of major atmospheric pollutants and visualizes them using the **Google Earth Engine UI**.

The application lets users explore pollutants over time using a **dynamic weekly DateSlider**, layered visualization controls, and an integrated legend system.
**1. Multi-pollutant Weekly Air Quality Visualization**
The dashboard displays weekly averages of:

| Pollutant / Variable | Data Source | Band Used |
|---------------------|-------------|-----------|
| Aerosol Index | S5P AER_AI | `absorbing_aerosol_index` |
| Carbon Monoxide (CO) | S5P CO | `CO_column_number_density` |
| Ozone (O₃) | S5P O3 | `O3_column_number_density` |
| Nitrogen Dioxide (NO₂) | S5P NO2 | `tropospheric_NO2_column_number_density` |
| Sulfur Dioxide (SO₂) | S5P SO2 | `SO2_column_number_density` |
| Formaldehyde (HCHO) | S5P HCHO | `tropospheric_HCHO_column_number_density` |
| Methane (CH₄) | S5P CH4 | `CH4_column_volume_mixing_ratio_dry_air` |
| Cloud Fraction | S5P CLOUD | `cloud_fraction` |

---

## 🗺️ **2. Interactive Map Interface**
- Google Earth Engine Map UI
- Layer toggles for each pollutant
- High-quality scientific color palettes (Jet, Inferno, BrBG, Ice)
- Automatic weekly composite generation

---

## 🎚️ **3. Dynamic DateSlider**
- Selects **weekly time periods**
- Automatically filters images
- Updates all pollutant visualizations at once

---

## 🎨 **4. Custom Legend Panel**
- Auto-generated color bars
- Min–Mid–Max labels
- Category-wise legends for each pollutant
- Styled title and footnote

---

## 🗂️ **5. Region of Interest**
The analysis is clipped using a **boundary shapefile**:
