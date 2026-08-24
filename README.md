# 🌍 Map Location Extractor

> **Paste any URL returning location JSON data, instantly visualize markers on an interactive map, and auto-fill missing Street View data with zero backend hassle!**

[GitHub Repository / Live Demo](https://www.google.com/search?q=%23) · **v0.1** · *Human Prompted, AI Crafted*

---

## 🔥 Why Map Location Extractor?

Managing map coordinates and street view panorama IDs (`panoId`) across different APIs can be tedious and frustrating. **Map Location Extractor** is a lightweight, 100% client-side tool built to make extracting, inspecting, and enriching geographic JSON datasets effortless.

Whether you're building custom maps for geography guessing games (like *WorldGuessr* or *Geoguessr*) or visualizing public spatial data, this tool streamlines your workflow in seconds.

---

## ✨ Key Features

* **🔍 Universal JSON Parsing:** No matter what format or nested structure your API returns, the app automatically recursively scans arrays and objects to pinpoint latitudes and longitudes.
* **⚡ Smart Auto-Fill (Pano ID & Date):** Automatically fetch missing Street View panorama IDs and capture dates. Works out-of-the-box in **No-Key Mode**, or plug in your own official Google Maps API key.
* **🗺️ Interactive Dark-Themed Map:** Powered by **Leaflet** and **MarkerCluster**, featuring a sleek dark CARTO basemap.
* 🟢 **Green Markers:** Have full panorama data.
* 🔴 **Red Markers:** Missing panorama data (ready for auto-fill).


* **📦 Quick Export & Filtering:** Instantly filter markers by keyword, preview raw JSON responses, and download clean, standardized Map JSON files with a single click.

---

## 🚀 Quick Start / Usage

1. **Paste URL:** Enter any endpoint returning location JSON data into the landing page input.
2. **Inspect & Search:** View the automatically detected format, examine markers on the map, or use the sidebar search bar to filter locations.
3. **Enrich & Export:** Enable **Auto-fill** to fill in missing metadata, then hit **Download JSON** to get your ready-to-use map file!

---

```json
// Example of the clean exported Map JSON format:
{
  "name": "my-custom-map",
  "customCoordinates": [
    {
      "lat": 37.7749,
      "lng": -122.4194,
      "heading": 0.001,
      "pitch": 0,
      "zoom": 0.17,
      "extra": {
        "panoId": "CAoSLEFGMVFpcE...",
        "panoDate": "2023-05"
      }
    }
  ]
}

```

---

### ⚠️ Technical Note & Disclaimer

* **CORS Support:** The tool fetches directly from your browser; ensure target endpoints permit CORS requests.
* **Independent Project:** This is an independent open-source technical helper tool and is not affiliated with or endorsed by Geoguessr or WorldGuessr.
