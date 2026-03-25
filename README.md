# Landslide Exposure Database (LED)

**Analysis Framework for National Building-Level Study: Landslide Exposure in the United States**

This repository contains the analysis pipeline and code used to develop the **Landslide Exposure Database (LED)**. The LED is an integrated, high-resolution building inventory designed to characterize the physical and social dimensions of landslide exposure across the conterminous United States, Alaska, and Hawaii.

## Overview
Traditional landslide risk assessments often rely on coarse administrative aggregates. This project introduces a multi-scale framework that integrates physical terrain susceptibility with granular human geography. By unifying 128 million building footprints with population and socioeconomic attributes, the LED enables a precise understanding of how physical hazards intersect with social vulnerability.
* Data sources can be downloaded using Jupyter notebooks found in the [0_Input](0_Input/) folder.
* Methodology described can be completed using Jupyter notebooks found in the [1_Process](1_Process/) folder.
* Results are found in [2_Output](2_Output/) folder, which contains figure outputs.



## Key Features
* **Integrated Building Inventory:** A unified dataset created by merging National Structure Inventory (NSI) point data and Overture building footprints.
* **Multi-Scale Spatial Analysis:** Automated workflows for spatially joining building records to physiographic divisions, census tracts, and urban/rural designations.
* **Socioeconomic Characterization:** Integration of Community Resilience Estimates (CRE) and American Community Survey (ACS) indicators to evaluate differential resilience.
* **Population Scaling:** Implementation of a dasymetric mapping approach to scale building-level population estimates (derived from NSI) to match official census totals.
* **Validated Impact Records:** Includes methodologies for verifying historical landslide impacts through manual textual review and post-event satellite imagery (e.g., Hurricane Helene).



## Methodology
The development of the LED follows a three-step process:

1. **Inventory Creation (Step 1):** Integration of NSI and Overture data involving spatial matching, filtering algorithms, and machine learning classification of ambiguous structures.
2. **Geographic Classification (Step 2):** Assignment of buildings to physiographic and administrative units (states, census tracts, and urban/rural blocks) to facilitate multi-scale analysis.
3. **Socioeconomic Attribution (Step 3):** Linking building records to tract-level resilience markers and performing population scaling to ensure administrative consistency.



## Technical Stack
* **Core Languages:** Python (GeoPandas, Pandas, NumPy)
* **Geospatial Tools:** QGIS / ArcGIS Pro
* **Primary Data Sources:** National Structure Inventory (NSI), USGS, NOAA, U.S. Census Bureau, and Overture Maps Foundation.



---
*This project is part of a PhD dissertation at the University of Washington, Seattle, focusing on characterizing the physical and social dimensions of landslide exposure. Development herein is under review for initial submission in a journal paper. We reserve the privacy of the repository until publication.*
