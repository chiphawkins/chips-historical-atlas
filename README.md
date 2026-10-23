# Historical Atlas — first working prototype

Open `index.html` in a browser with an internet connection. It uses Leaflet 1.9.4, modern country polygons from Natural Earth via `datasets/geo-countries`, and time-indexed historical GeoJSON from André Ourednik's `historical-basemaps` repository.

Three separate map layers are present: physical basemap tiles, contemporary country outlines/US-English labels, and historical polygons/labels. The timeline chooses the most recent available historical snapshot at or before the chosen year; it does **not** invent intermediate borders.

## Hosting

Upload `index.html` to GitHub Pages, Netlify, or any static web server. No build tools are needed. A network connection is required for map tiles, JS libraries, and GeoJSON data. For production, cache/pin source datasets, host files yourself, and add rigorous historical attribution, feature-level dating, a source-confidence system, and historical administrative-level datasets.

## Important limitations

The historical source is GPL-3.0 and its author warns it is work in progress. It does not reliably include all kingdoms, duchies, principalities, and city-states in all periods. The modern country names are normalized toward US English; some Natural Earth labels and cartographic choices may require editorial review. The map's physical basemap represents current geography, not reconstructed historical coastlines.
