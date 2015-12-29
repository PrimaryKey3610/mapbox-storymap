# mapbox-storymap
Scroll-driven storymap with narrative and point markers, using Mapbox GL and Mapbox.js

## Best demo (using Mapbox GL)
http://jackdougherty.github.io/mapbox-storymap/index.html

## see also regular mapbox demos
http://jackdougherty.github.io/mapbox-storymap/markers.html

http://jackdougherty.github.io/mapbox-storymap/pulse.html

## Dependency
requires a Mapbox account token (free up to 50,000 views per month)

## Credits
Mapbox GL story map with scroll fly-to https://www.mapbox.com/mapbox-gl-js/example/scroll-fly-to/

Mapbox GL story map (Madrid airport runway) https://www.mapbox.com/bites/00045/

Mapbox storymap tutorial (Sherlock Holmes) (https://www.mapbox.com/mapbox.js/example/v1.0.0/scroll-driven-navigation/

## To Do
- test older IE browser support and older iPad browsers
- define all points, refer to them in chapters, and display all at start and during storymap
  - this is a real pain in MapBoxGL: https://www.mapbox.com/mapbox-gl-js/example/geojson-markers/
  - is there a MapboxGL equivalent to:
    - L.marker([38.913184,-77.031952]).addTo(map);
- evaluate pros and cons of one-color markers vs changing color when featured in narrative (see prior version)
- determine if it will display polygons (as geojson objects?) for narratives about boundaries
- need code to automatically resize and center images to fit narrative div width (as in pulse version)
