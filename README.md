# Visualizing Boston's Bike Share Network
### DSC 106 Project @ UCSD

**An interactive geospatial visualization of the BlueBikes network, revealing the "pulse" of Boston's commute patterns through data.**

🚲 <a href="https://musubi3.github.io/boston-bike-watching/" target="_blank"><strong>View Live Visualization</strong></a>

---

## 📊 Project Overview
Boston runs on BlueBikes, but static maps don't capture how the city moves. This project brings the network to life by visualizing over **260,000 individual trips** from March 2024.

By animating traffic flow over a 24-hour cycle, we can see the city "breathe":
1.  **Morning Rush:**<br>Commuters flood into Kendall Square and Financial District (Blue departures → Orange arrivals).<br><br>
2.  **Evening Reversal:**<br>The pattern flips as riders leave commercial hubs to return to residential neighborhoods.<br><br>
3.  **The "Pulse":**<br>Station markers swell and shrink in real-time to reflect total traffic volume, while colors shift to indicate whether a station is a "source" (more departures) or a "sink" (more arrivals).

---

## 🛠️ Tech Stack
* **Core Libraries:**<br>Mapbox GL JS, D3.js (v7).<br><br>
* **Frontend:**<br>HTML5, CSS3.<br><br>
* **Data Format:**<br>GeoJSON (Bike Lanes) & CSV (Trip Data).

---

## 📂 Data Sources
| Dataset | Source | Description |
| :--- | :--- | :--- |
| **BlueBikes Trip Data** | [BlueBikes System Data](https://www.bluebikes.com/system-data) | Comprehensive ride data from **March 2024**, containing start/end times and station IDs. |
| **Station Metadata** | [BlueBikes API](https://gbfs.bluebikes.com/gbfs/gbfs.json) | Real-time station status including coordinates and capacity (snapshot). |
| **Bike Lanes** | [Boston Open Data](https://data.boston.gov/) | Geospatial lines representing existing bike infrastructure in Boston and Cambridge. |