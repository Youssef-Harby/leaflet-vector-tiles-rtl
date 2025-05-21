# Leaflet Vector Tiles with MapLibre GL

A simple implementation of vector tile maps using Leaflet with MapLibre GL integration.

## Overview

This project demonstrates how to use vector tiles in a Leaflet map using the MapLibre GL library for rendering. It includes support for RTL (Right-to-Left) text rendering for languages like Arabic.

## Features

- Vector tile rendering with Leaflet
- MapLibre GL integration for better vector tile handling
- RTL text support for Arabic and other right-to-left languages
- Responsive and fullscreen map

## Getting Started

### Prerequisites

No installation required. All dependencies are loaded from CDNs.

Then open your browser and navigate to `http://localhost:8000`.

## Technologies Used

- [Leaflet](https://leafletjs.com/) - The core mapping library
- [MapLibre GL JS](https://maplibre.org/) - For vector tile rendering
- [MapLibre GL Leaflet](https://github.com/maplibre/maplibre-gl-leaflet) - Integration between Leaflet and MapLibre GL

## Configuration

The map is configured to use OpenStreetMap Japan vector tiles by default. You can modify the style URL in the `index.html` file to use different vector tile sources.

```javascript
const vectorTileLayer = L.maplibreGL({
    style: 'https://tile.openstreetmap.jp/styles/openmaptiles/style.json',
    attribution: '© <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
}).addTo(map);
```