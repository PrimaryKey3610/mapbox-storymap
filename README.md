# mapbox-storymap
Scroll-driven storymap with narrative and point markers, using Mapbox GL

## Demos
http://jackdougherty.github.io/mapboxgl-storymap/index.html

## see also regular mapbox demos
http://jackdougherty.github.io/mapbox/index-markers.html

http://jackdougherty.github.io/leaflet-storymap-mapbox/index-pulse.html

## Dependency
requires a Mapbox account token (free up to 50,000 views per month)

## Credits
Mapbox GL story map with scroll fly-to https://www.mapbox.com/mapbox-gl-js/example/scroll-fly-to/

Mapbox GL story map (Madrid airport runway) https://www.mapbox.com/bites/00045/

Mapbox storymap tutorial (Sherlock Holmes) (https://www.mapbox.com/mapbox.js/example/v1.0.0/scroll-driven-navigation/

## To Do
- test benefits of MapBox dependency (such as high-quality satellite imagery?)
- test older IE browser support and older iPad browsers
- try making pure Leaflet version with map.flyTo in beta 1.0
- define all points, refer to them in chapters, and display all at start and during storymap
    this is a real pain in MapBoxGL: https://www.mapbox.com/mapbox-gl-js/example/geojson-markers/
    if portable to pure Leaflet, try this:
    L.marker([38.913184,-77.031952]).addTo(map);
    L.marker([37.775408,-122.413682]).addTo(map);
- evaluate pros and cons of one-color markers vs changing color when featured in narrative (see prior version)
- determine if it will display polygons (as geojson objects?) for narratives about boundaries
- Ask MAGIC: need code to automatically resize and center images to fit narrative div width (as in pulse version)
