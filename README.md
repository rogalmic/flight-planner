# VFR Flight Planner

![Flight planner](./img/flight_planner.png "Flight planner")

## Features

* Flight planning with wind and magnetic declination correction with greart circle path for longer routes
* Output in `km/h`, `km` or `nm`, `kts`, input via selection of value (both unit systems shown)\
![Input units](./img/units.png "Input units")
* Background map png tiles in `EPSG:3857` format, like from https://www.openflightmaps.org/ (possibility to download ~1GB zip with tiles for given region, then paste `slippyTiles_original.zip\original\merged\256\latest` contents to local `./tiles` folder)
  * Default remote tiles from `https://{a-c}.tile.openstreetmap.org/{z}/{x}/{y}.png`, possibility to change via `?remote_tile_url=...` \
![OSM remote tiles](./img/osm_tiles.png "OSM tiles")
  * Default local tiles from `./tiles/{z}/{x}/{y}.png`, possibility to change via `?local_tile_url=...` \
![Custom local tiles](./img/custom_tiles.png "Custom local tiles")
  * Possibility to switch between `local`/`remote` background maps during planning route
  * Remote maps work out-of-the-box, while local maps require setup
* Open `METAR` and `TAF` for given route in separate page (https://aviationweather.gov/adds/), follows great circle path
* Export plan to [CSV file](https://en.wikipedia.org/wiki/Comma-separated_values) for further adjustments in external tools

## Samples

* [OSM MAP VERSION](https://rogalmic.github.io/flight-planner/flight.html?log_units=metric)
* [OSM MAP VERSION (results in nm and kts, US centered)](https://rogalmic.github.io/flight-planner/flight.html?log_units=alternative&z=5&lon=-97.479&lat=39.408)
* [WIKIMEDIA MAP VERSION](https://rogalmic.github.io/flight-planner/flight.html?remote_tile_url=https%3A%2F%2Fmaps.wikimedia.org%2Fosm-intl%2F%7Bz%7D%2F%7Bx%7D%2F%7By%7D.png)
* [NO LABELS MAP VERSION](https://rogalmic.github.io/flight-planner/flight.html?remote_tile_url=https%3A%2F%2Ftiles.wmflabs.org%2Fosm-no-labels%2F%7Bz%7D%2F%7Bx%7D%2F%7By%7D.png)

## Objectives

* as simple as possible with interaction options at every step, nothing purely automatic
* based on OSM, but with possibility to change to different source
* remember offline data in `tiles` folder, see https://github.com/hdjarv/osm-tile-downloader, offline deliverable built in `travis`

## Requirements

* recent browser with support for `HTML5` and `ECMAScript 2015`

## Dev Requirements

* Really easy, just try :)
* `Visual Studio Code`
* `Git`
* `Debugger for Chrome` or `Debugger for Chrome` VsCode extension

 1. Get repo \

```shell
git clone "https://github.com/rogalmic/flight-planner.git"
code "./flight-planner/"
```
 2. Select debug option (chrome or firefox)
 3. Run debug session
 4. Optionally load tiles in proper folder structure to `./tiles/{z}/{x}/{y}.png` (`EPSG:3857` format)
