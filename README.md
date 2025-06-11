# 🌐 QuakeTrack: End-to-End Earthquake Analytics with Microsoft Fabric

## 📖 Project Overview

**QuakeTrack** is a full-scale data engineering and analytics project built using **Microsoft Fabric** that ingests real-time earthquake event data from the [USGS Earthquake API](https://earthquake.usgs.gov/fdsnws/event/1/#parameters), processes it through structured Bronze, Silver, and Gold layers using PySpark notebooks, and visualizes insightful metrics using Power BI.

This project demonstrates the complete lifecycle of modern data engineering using **Microsoft Fabric’s unified Data Factory, Lakehouse, and Power BI experiences**.

---

## 🛠️ Technologies Used

- **Microsoft Fabric**
  - Data Engineering (Lakehouse, Notebooks)
  - Data Factory (Pipeline orchestration)
  - Power BI (Reporting)
- **PySpark** (inside Fabric notebooks)
- **USGS Earthquake API** (data source)
- **OneLake** (storage and querying)

---

## 🚀 Getting Started

To explore or replicate this project:

1. Clone/download this repository.
2. Open Microsoft Fabric.
3. Import the notebooks into your workspace.
4. Set up the Lakehouse storage named `earthquake_lakehouse`.
5. Use the provided data pipeline to orchestrate the flow.
6. Connect Power BI to the curated data for dynamic visualizations.

---

## 📂 Repository Contents

| File | Description |
|------|-------------|
| `Earthquake Events Bronze Layer.ipynb` | Ingests raw earthquake data from USGS API and stores it in Lakehouse. |
| `Earthquake Events Silver Layer.ipynb` | Cleans, transforms, and enriches Bronze data for analytical readiness. |
| `Earthquake Events Gold Layer.ipynb` | Refines Silver data into a business-ready format for reporting. |
| `PowerBI_Report.pdf` | Static version of the Power BI dashboard for quick review. |

---

## 🧬 Data Attribute Definitions

| Column | Description |
|--------|-------------|
| `id` | Unique identifier for the earthquake event |
| `latitude` | Geographic latitude of the event |
| `longitude` | Geographic longitude of the event |
| `elevation` | Elevation above sea level (in meters) |
| `title` | Full description/title of the event |
| `place_description` | Human-readable location string |
| `sig` | Significance score representing event severity |
| `mag` | Magnitude of the earthquake |
| `magType` | Type of magnitude scale used |
| `time` | Timestamp when the earthquake occurred |
| `updated` | Timestamp when the record was last updated |

---

## 🔁 Pipeline Execution (Fabric Data Factory)

![Pipeline](./Screenshot%202025-06-11%20103022.png)

The project uses a 3-stage Fabric pipeline:
1. **Bronze Notebook** → Raw ingestion.
2. **Silver Notebook** → Cleansing & transformation.
3. **Gold Notebook** → Final analytical dataset creation.

✅ Status: All stages **succeeded**

---

## 📊 Power BI Dashboard

📍 Visualized earthquake data by:
- Magnitude
- Region
- Time (monthly/yearly trends)
- Geospatial locations (lat/lon heatmaps)

📎 Preview (PDF): [`PowerBI_Report.pdf`](./PowerBI_Report.pdf)

---

## 💡 Highlights

- End-to-end ETL and visualization pipeline on Microsoft Fabric
- Real-time ingestion of natural disaster data
- Scalable and modular notebook design
- Production-grade reporting with Power BI

---

## 🧑‍💻 Author

**Saipradeep Bomma**  
📍 Dallas, TX  
📫 saipradeepbomma16@gmail.com  
🔗 [GitHub](https://github.com/saipradeep16) | [LinkedIn](https://www.linkedin.com/in/saipradeepbomma16)
