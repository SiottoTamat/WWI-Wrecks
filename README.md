# WWI Shipwrecks Dataset

This repository contains a curated list of naval shipwrecks that occurred during World War I. It includes both a tabular CSV format and a geographic GeoJSON format for ease of analysis and visualization.

## Repository Structure

```
WWI-Shipwrecks/
│
├── data/
│   ├── DB_WWI_Wrecks.csv      # Tabular data of WWI shipwrecks
│   └── DB_WWI_Wrecks.geojson  # Geographic data of WWI shipwrecks
```

## Data Description

Each record represents a shipwreck event, with the following fields:

| Field       | Description                                                                          |
|-------------|--------------------------------------------------------------------------------------|
| Index       | Unique identifier for the entry                                                     |
| Name        | Name of the ship                                                                    |
| Date        | Date of the shipwreck event (format: DD/MM/YYYY)                                    |
| Longitude   | Longitude of the wreck site                                                         |
| Latitude    | Latitude of the wreck site                                                          |
| Navy        | The navy or country to which the ship belonged                                      |
| Description | A brief description of the shipwreck event                                          |
| Cause       | The primary cause of the wreck (e.g. torpedo, mine, explosion, weather, unknown)    |

## Formats

- **CSV** (`DB_WWI_Wrecks.csv`): Plain text format suitable for spreadsheets and data processing tools. (with events of unknown coordinates)
- **GeoJSON** (`DB_WWI_Wrecks.geojson`): Geospatial format for use with GIS software and web mapping platforms. (without events of unknown coordinates)

## Example Entry

```json
{
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [55.98944, 17.76028]
  },
  "properties": {
    "Index": "0",
    "Name": "SMS G143",
    "Date": "03/08/1914",
    "Navy": "Kaiserliche Marine",
    "Description": "The S138-class destroyer suffered a boiler explosion and sank in the Baltic Sea.",
    "Cause": "explosion/fire"
  }
}
```

## Purpose

This dataset is intended for:
- Historical research
- Maritime archaeology
- Educational projects
- GIS visualization and spatial analysis

## License

This dataset is shared under a permissive license. Please credit appropriately if you reuse it. For questions or contributions, feel free to open an issue or pull request.

---

Curated by Andrea Siotto
