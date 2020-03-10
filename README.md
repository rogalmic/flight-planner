# flight-planner

* Flight Planner
 - [OSM MAP VERSION](https://rogalmic.github.io/flight-planner/flight.html?log_units=metric)
 - [OSM MAP VERSION (results in nm and kts, US centered)](https://rogalmic.github.io/flight-planner/flight.html?log_units=alternative&z=5&lon=-97.479&lat=39.408)
 - [WIKIMEDIA MAP VERSION](https://rogalmic.github.io/flight-planner/flight.html?remote_tile_url=https%3A%2F%2Fmaps.wikimedia.org%2Fosm-intl%2F%7Bz%7D%2F%7Bx%7D%2F%7By%7D.png)
 - [NO LABELS MAP VERSION](https://rogalmic.github.io/flight-planner/flight.html?remote_tile_url=https%3A%2F%2Ftiles.wmflabs.org%2Fosm-no-labels%2F%7Bz%7D%2F%7Bx%7D%2F%7By%7D.png)

OBJECTIVES:
- as simple as possible with interaction options at every step, nothing purely automatic
- based on OSM, but with possibility to change to different source
- remember offline data in `tiles` folder, see https://github.com/hdjarv/osm-tile-downloader, offline deliverable built in `travis`

Requirements:
- recent browser

Dev Requirements:
- `Visual Studio Code`
- `Debugger for Chrome` or `Debugger for Chrome` VsCode extension