# Nickel Exploration Potential in Ontario, Canada

This project is a GIS and Python-based exploratory study of nickel exploration potential in Ontario, Canada.  
It uses open geoscience data from the Ontario Mineral Inventory and the Bedrock Geology of Ontario to identify districts where nickel occurrences, favourable lithologies and mining maturity overlap.

## Objective

The objective is to build a first spatial prioritization of nickel exploration potential in Ontario using open data.

The study does not estimate the economic value of deposits.  
It ranks districts according to relative exploration potential based on:

- nickel occurrences from the Ontario Mineral Inventory;
- mining status of each occurrence;
- location on mafic and ultramafic rocks;
- district-level scoring;
- reproducible Python processing.

## Data Sources

- Ontario Mineral Inventory — GeologyOntario  
- Bedrock Geology of Ontario, MRD126-REV1 — GeologyOntario  
- Ontario GeoHub — administrative boundaries  
- OpenStreetMap — basemap used in QGIS  

## Methodology

The workflow follows five main steps:

1. Extract nickel occurrences from the Ontario Mineral Inventory.
2. Identify mafic and ultramafic geological units from the Bedrock Geology of Ontario.
3. Select nickel occurrences intersecting favourable lithologies.
4. Build a district-level exploration score based on mining status.
5. Use Python to verify the results and calculate complementary indicators.

## Key Results

The initial extraction identified **1,554 nickel occurrences** in Ontario.

A geological filter was then applied to retain only nickel occurrences located on mafic or ultramafic rocks.  
This produced **589 favourable occurrences**, representing about **37.9%** of all nickel occurrences.

The final district ranking is:

| Rank | District | Favourable occurrences | Final score | Class |
|---:|---|---:|---:|---|
| 1 | Sudbury | 162 | 278 | Very high |
| 2 | Kirkland Lake | 100 | 220 | High |
| 3 | Timmins | 141 | 193 | High |
| 4 | Thunder Bay South | 59 | 74 | Intermediate |
| 5 | Thunder Bay North | 34 | 45 | Intermediate |
| 6 | Kenora | 31 | 36 | Moderate |
| 7 | Red Lake | 32 | 35 | Moderate |
| 8 | Southern Ontario | 17 | 22 | Low |
| 9 | Sault Ste. Marie | 13 | 16 | Low |

## Main Interpretation

Sudbury appears as the most robust district because it combines:

- a high number of nickel occurrences on favourable rocks;
- advanced mining status;
- strong geological consistency.

Kirkland Lake ranks above Timmins despite fewer favourable occurrences, because its average maturity index is higher.  
Timmins remains important in volume, but its average maturity profile is lower.

## Python Contribution

Python was used to make the scoring reproducible and to calculate additional indicators:

- share of favourable occurrences by district;
- share of total score by district;
- maturity index.

The maturity index is calculated as:

```text
maturity index = final score / favourable occurrences
