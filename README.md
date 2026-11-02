# Aspen CSG Hub Map: geography prototype

An interactive prototype of how the Rural Development Hubs map shows states, regions, a selected Hub's footprint and the tribal lands reference layer, built inside the approved Concept 3 design.

**Live prototype:** after GitHub Pages is turned on, it lives at `https://<account>.github.io/<repo>/`.

## How to review
1. Use the yellow **Scenario** bar to step through the key states:
   - Default
   - Appalachia
   - Appalachia + MDC
   - Indigenous-serving, with and without a Hub selected
   - Three overlapping layers
2. The map uses one consistent treatment for overlapping layers: a cased boundary for the selected state or region, and a hatched footprint for the selected Hub.
3. The **System**, **Interactions** and **Implementation** tabs explain the visual rules, the interaction behavior and the build approach.
4. Everything is clickable: states on the map, the tabs, the menus, search, the Indigenous-serving toggle, the Hub rows, Hide and Reset map.

## Data
- **States:** U.S. Census cartographic boundaries (us-atlas 3.0.1, Albers USA).
- **Appalachia:** merged Census county shapes for the Appalachian Regional Commission's counties, plus 8 Virginia independent cities.
- **Tribal lands:** U.S. Census Bureau TIGERweb AIANNH layers. Reservations and trust lands are shown separately from statistical areas. They are reference geography, not Hub service areas.
- **Hub names and states:** from the current aspencsg.org map.
- **Provisional until the Hubs spreadsheet is connected:**
  - Indigenous-serving status
  - region membership
  - funders
  - most descriptions
- **Illustrative only:** the "Stress test" scenario uses a clearly labeled sample Hub that is not real data.

## Technical notes
This is a single static `index.html` with the geography embedded. It loads one small library (topojson-client) from jsDelivr. There's no build step, server or API key.
