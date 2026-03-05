# Housing Price and Volume — Indonesia 🇮🇩

Exploratory and spatial analysis of residential property listings across 14 major Indonesian cities. Built as part of the **Datakota Urban Data Scientist Assessment (2025)**.

---

## Overview

This project investigates **spatial price gradients and listing concentration patterns** across Indonesia's major metropolitan areas — with a deep-dive into DKI Jakarta at kecamatan (sub-district) level.

The notebook is structured as an analytical essay: each section builds on the previous, moving from broad market structure to granular geographic insights and actionable strategic signals.

| Layer | Question | Section |
|-------|----------|---------|
| Market Structure | What does the overall price distribution look like? | Section 2 — EDA |
| Spatial Gradient | Where do prices concentrate geographically? | Section 3 — Geospatial |
| Demand Driver | What explains price variation? | Section 4 & 6 |
| Strategic Signal | Where are the underpriced, high-opportunity markets? | Section 6.3 |

---

## Key Analyses

- **Exploratory Data Analysis** — price distribution, outlier detection, city-level benchmarking, district-level ranking across 14 cities
- **DKI Jakarta Choropleth** — 3-panel kecamatan-level map: land price per m², median listing price, listing volume
- **Population Density Integration** — testing the density-price relationship using 2024 DKI Jakarta government data
- **Housing Affordability Map** — years of UMP (minimum wage) needed to afford a house per kecamatan
- **MRT Proximity Premium** — does transit infrastructure inflate land values? Phase 1 & 2 station analysis
- **Market Opportunity Quadrant** — 2×2 strategic matrix identifying underpriced high-demand kecamatan

---

## Dataset

| Dataset | Source |
|---------|--------|
| Housing listings (1,817 rows, 14 cities) | Provided — Datakota Assessment |
| Kecamatan boundaries | Badan Informasi Geospasial (BIG) |
| Population density (2024) | Jakarta Open Data Portal — data.jakarta.go.id |
| UMP DKI Jakarta 2024 | Pergub DKI Jakarta No. 57 Tahun 2023 |
| MRT station coordinates | PT MRT Jakarta — mrtjakarta.com |

---

## Project Structure

```
housing_project/
├── notebook/
│   └── Report_Notebook_Final.ipynb   ← main submission
├── urbandatascientisttakehometest/
│   └── Housing Price & Volume.csv    ← raw dataset (not tracked)
├── Data/
│   ├── Data DKI Jakarta/             ← external datasets (not tracked)
│   ├── batas_administrasi/           ← boundary shapefiles (not tracked)
│   └── output/                       ← geocoded data & basemap (not tracked)
├── output/                           ← exported charts & maps
├── requirements.txt
├── .gitignore
└── README.md
```

---

## Requirements

Install dependencies:

```bash
pip install -r requirements.txt
```

Core libraries used:

```
pandas
numpy
matplotlib
seaborn
geopandas
shapely
geopy
```

---

## How to Run

1. Clone the repository
2. Install requirements
3. Open `notebook/Report_Notebook_Final.ipynb`
4. Update file paths at the top of the notebook to match your local directory
5. Run All cells

---

## License

MIT License — see `LICENSE` for details.
