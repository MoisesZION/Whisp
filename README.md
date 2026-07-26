# WHISP - Local OpenForis WHISP Workflow

This repository contains a local implementation of the **OpenForis WHISP** workflow using **Google Earth Engine** and Python.

The project reproduces the official WHISP notebook while allowing the analysis of custom GeoJSON files without using the online interface.

---

## Project Structure

```text
WHISP/
│
├── data/
│   ├── input/
│   │   └── *.geojson
│   │
│   └── outputs/
│       ├── csv/
│       └── geojson/
│
├── notebooks/
│   └── whisp_geojson_to_csv.ipynb
│
├── .gitignore
├── README.md
└── requirements.txt
```

---

## Features

- Authenticate with Google Earth Engine
- Load custom GeoJSON files
- Build the WHISP multiband image
- Compute WHISP statistics
- Calculate risk indicators
- Export results to CSV
- Export enriched GeoJSON

---

## Requirements

- Python 3.13+
- Google Earth Engine account
- Google Cloud Project registered for Earth Engine
- OpenForis WHISP

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Input

Place the GeoJSON to be analyzed inside:

```text
data/input/
```

---

## Output

Results are automatically exported to:

```text
data/outputs/csv/
```

and

```text
data/outputs/geojson/
```

---

## Workflow

```text
GeoJSON
    │
    ▼
Google Earth Engine
    │
    ▼
OpenForis WHISP
    │
    ▼
Statistics
    │
    ▼
Risk Assessment
    │
    ├── CSV
    └── GeoJSON
```

---

## Reference

Official OpenForis WHISP repository:

https://github.com/forestdatapartnership/openforis-whisp

---

## Current Status

✅ Earth Engine authentication

✅ Local execution of OpenForis WHISP

✅ Custom GeoJSON processing

✅ CSV export

✅ GeoJSON export

---

## Future Work

- Improve notebook documentation
- Explore WHISP output variables
- Integrate additional Colombian datasets
- Develop reusable workflows for spatial analysis