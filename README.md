# mapbox-storymap
Scroll-driven storymap with narrative and point markers, using Mapbox GL and Mapbox.js

## Best demo (using Mapbox GL)
http://jackdougherty.github.io/mapbox-storymap/index.html

### Benefits:
- Clean scroll-driven navigation
- Users can pan and zoom map independently from scroll navigation to explore further
- Mapbox GL supports decimal zoom levels (e.g. 13.5, and also pitch and bearing)

## see also regular Mapbox.js demos
http://jackdougherty.github.io/mapbox-storymap/markers.html

http://jackdougherty.github.io/mapbox-storymap/pulse.html

## Dependency
requires a Mapbox account token (free up to 50,000 views per month)

MapboxGL is supported by all modern browsers (Chrome, FFox, Safari) and Internet Explorer 9+

Note: When testing Apple iPad 1st generation with most recent Safari and Chrome available on that device, the code displayed the alert message, "Your browser does not support Mapbox GL".

## Credits
Mapbox GL story map with scroll fly-to https://www.mapbox.com/mapbox-gl-js/example/scroll-fly-to/

Mapbox GL story map (Madrid airport runway) https://www.mapbox.com/bites/00045/

Mapbox storymap tutorial (Sherlock Holmes) (https://www.mapbox.com/mapbox.js/example/v1.0.0/scroll-driven-navigation/

## To Do
- define all points, refer to them in chapters, and display all at start and during storymap
  - this is a real pain in MapBoxGL: https://www.mapbox.com/mapbox-gl-js/example/geojson-markers/
  - is there a MapboxGL equivalent to:
    - L.marker([38.913184,-77.031952]).addTo(map);
- display third-party tileLayers (such as CartoDB LightAll and CT Aerial 1934 WMS)
- evaluate pros and cons of one-color markers vs changing color when featured in narrative (see prior version)
- determine if it will display polygons (as geojson objects?) for narratives about boundaries
- need code to automatically resize and center images to fit narrative div width (as in pulse version)
- ask Mapbox support: when testing IE 8, my browser support code alert did not appear, even though it's based on the same code as this sample that correctly displays, with a reminder to update IE (https://www.mapbox.com/mapbox-gl-js/example/check-for-support/)
