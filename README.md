# ForD: Global Forest Disturbance Database

ForD is a global database of documented intermediate-scale forest biomass loss events and their proximate and exacerbating drivers. Records were compiled from the primary scientific literature and represent individual mortality events with elevated biomass loss (typically ≥15% annual mortality) occurring after the year 2000.

## Associated manuscript

This database was compiled as part of a global review of drivers of forest biomass loss:

> [Authors]. (*in preparation*). Global drivers and mitigation of forest biomass loss. *[Global Change Biology]*. DOI: [placeholder]

## Database contents

`ForD.csv` contains records of forest biomass loss events from across the globe. Each row represents a documented mortality event at a single site. Fields include:

- **Location**: latitude and longitude (decimal degrees)
- **Coordinate precision**: how precisely the location is known
- **DriverGroup**: standardized driver category assigned from the primary proximate driver
- **Citation key**: Zotero-formatted key linking to the source study
- **DOI**: digital object identifier of the source study

See `metadata.csv` for full field definitions and `data_procedure.md` for the inclusion criteria and driver classification scheme used to compile the database.

## Driver category scheme

The `DriverGroup` field assigns each record to one of the following categories based on its primary proximate driver:

| DriverGroup |
|---|
| heat and drought |
| storms |
| biotic disturbance |
| wildfire |
| fuelwood harvest |
| logging & forestry |
| permanent agriculture |
| shifting agriculture |
| mining & energy |
| settlements & infrastructure |
| permafrost thaw |
| other |

## Data citation

If you use this database, please cite:

> [Authors]. (*in preparation*). ForD: Global Forest Disturbance Database (v1.0). Zenodo. DOI: [placeholder]

## License

This dataset is released under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
