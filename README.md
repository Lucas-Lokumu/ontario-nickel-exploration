# Nickel Exploration Potential in Ontario, Canada

## Overview

This project is a data-driven exploratory study of nickel exploration potential in Ontario, Canada.

It combines public mining datasets, geological information, spatial analysis and economic interpretation to identify areas with stronger nickel exploration interest. The project was developed as a portfolio case study at the intersection of applied economics, natural resources, critical minerals and geospatial analysis.

The analysis focuses on nickel occurrences, mafic and ultramafic geological units, and spatial relationships that may indicate favourable exploration zones.

---

## Objectives

The main objectives of this project are:

- Identify and filter nickel-related mineral occurrences in Ontario
- Cross-reference nickel occurrences with favourable geological units
- Map spatial patterns using QGIS
- Highlight areas with stronger exploration potential
- Produce a clear analytical report in French and English
- Build a reproducible and documented portfolio project on critical minerals

---

## Data Sources

The project uses publicly available geological and mining data, mainly from Ontario open data sources.

Main datasets include:

- Ontario Mineral Inventory / OMI mineral occurrence data
- Geological layers related to mafic and ultramafic formations
- Processed nickel occurrence datasets
- Spatial layers used for QGIS mapping and interpretation

The dataset used in this repository is a processed version created for analytical and educational purposes.

---

## Methodology

The workflow follows several steps:

1. **Data collection**  
   Public mining and geological data were collected from Ontario open data sources.

2. **Nickel occurrence filtering**  
   The Ontario Mineral Inventory dataset was filtered to isolate nickel-related occurrences.

3. **Geological selection**  
   Mafic and ultramafic geological units were selected because they are commonly associated with nickel sulphide exploration contexts.

4. **Spatial overlay analysis**  
   Nickel occurrences were intersected or compared with favourable geological units to identify zones of stronger geological interest.

5. **Mapping in QGIS**  
   Maps were created to visualize:
   - Nickel occurrence distribution
   - Final nickel potential zones
   - Geological context

6. **Economic interpretation**  
   Results were interpreted from a natural resources and critical minerals perspective, with attention to exploration potential rather than mine valuation.

---

## Repository Structure

```text
ontario-nickel-exploration/
│
├── Rapport_Nickel_Ontario.pdf
├── Nickel_Ontario_Report_EN.pdf
├── Nickel_Ontario.qgz
├── OMI_nickel.shp.gpkg
├── omi_nickel_on_mafic_ultramafic.csv
├── carte_1_localisation_occurrences_nickel_ontario.png
├── carte_finale_potentiel_nickel_ontario.png
└── README.md
