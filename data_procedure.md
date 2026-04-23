# ForD Database: Compilation Procedure

This document describes the criteria and methods used to compile records in the ForD (Global Forest Disturbance) database.

## Inclusion criteria

Records document forest biomass loss events meeting all of the following criteria:

- The event involved **elevated tree mortality or significant biomass loss** (a working threshold of ~15% annual mortality, though quantitative measurement was not required)
- The event occurred **at or after the year 2000**
- The study provides **geographic coordinates** and at least one identified **proximate driver**
- "Forest decline" qualifies if elevated mortality is documented; decline in growth alone does not qualify
- Plantations and afforestation sites are included
- Studies documenting **forest area loss** are included without a quantitative threshold

## Literature search

Studies were identified through keyword searches of scientific literature databases and review of references within included papers. Only one row is entered per site per event; when a single paper reports multiple distinct sites, each site is entered as a separate row.

## Driver classification

Each record assigns **proximate drivers** and **exacerbating drivers** from a standardized vocabulary.

**Proximate driver** — the most immediate cause of tree death or biomass loss, identifiable in principle by field observation of affected trees:

> heat, drought, storm, storm (lightning), storm (wind), storm (hurricane), frost, insects, insects (endemic), insects (non-endemic), pathogen, pathogen (endemic), pathogen (non-endemic), fire, fire (wildfire), fire (anthropogenic management), fuelwood harvest, selective logging, forestry harvest, shifting cultivation, agriculture, pasture, mining, extraction, urban expansion, air pollution, water pollution, animals (livestock), animals (wild), other

**Exacerbating driver** — a factor that increases tree vulnerability to the proximate driver but does not directly cause mortality (same vocabulary as proximate drivers, with the addition of: competition, topographic position, soil type).

Classification notes:
- When bark beetles kill trees during drought, insects are the proximate driver and drought is an exacerbating driver
- Drought is defined as moisture stress from low precipitation or high vapor pressure deficit
- Storms include wind, rain, and lightning in any combination
- Events can have multiple proximate and exacerbating drivers; up to two of each are recorded in dedicated columns, with additional drivers in overflow fields

For use in analyses, `proximate.driver.1` is mapped to a standardized grouping column called **`DriverGroup`** (see `metadata.csv` for category definitions).

## Coordinates

Coordinates are recorded in decimal degrees (negative for S latitude and W longitude). The `coordinate.precision` field records how precisely the location is known (degree, minute, second, or decimal degrees to *n* digits). When only a regional range is reported, central coordinates are used. When results are differentiated across multiple plots within a study, each plot is entered as a separate row.
