# Aspen CSG Hub Map: geography prototype

An interactive prototype of the Rural Development Hubs map, built in the approved design. It shows how states, regions, a selected Hub's footprint and the tribal lands reference layer appear together.

**Live prototype:** https://liv610.github.io/aspen-hub-map/

## What to try
- Hover over and click states on the map, or choose a state from the menu.
- Open **Regions** and choose **Appalachia**, then select **MDC** in the results list. This shows a region and a multi-state Hub at the same time.
- Turn on **Indigenous-serving** to filter the Hubs and show the tribal lands reference layer.
- Use **Hide** on a Hub card or press **Esc** to return to the previous view, and **Reset map** to start over.

## Data
- **States:** U.S. Census cartographic boundaries.
- **Appalachia:** the Appalachian Regional Commission's counties, merged from Census county shapes.
- **Tribal lands:** U.S. Census Bureau TIGERweb. These are reference geography, not Hub service areas.
- **Hub names and states:** from the current aspencsg.org map.
- **Provisional until the Hubs spreadsheet is connected:**
  - Indigenous-serving status
  - region membership
  - funders
  - most descriptions

## Technical notes
This is a single static `index.html` with the geography embedded. It loads one small library (topojson-client) from jsDelivr. There's no build step, server or API key.
