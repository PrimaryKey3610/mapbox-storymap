# mapbox-storymap
Scroll-driven storymap with narrative and point markers, using Mapbox GL and Mapbox.js

## Demo (with Mapbox GL)
http://jackdougherty.github.io/mapbox-storymap/index.html

### Benefits:
- Clean scroll-driven navigation
- Users can pan and zoom map independently from scroll navigation to explore further
- Mapbox GL supports decimal zoom levels (e.g. 13.5, and also pitch and bearing)

## Other demos in this folder
- with Mapbox.js markers
http://jackdougherty.github.io/mapbox-storymap/markers.html

- with Mapbox.js pulse
http://jackdougherty.github.io/mapbox-storymap/pulse.html

- TESTING (not yet working) Leaflet-only version of Mapbox GL code (without Mapbox dependency)
http://jackdougherty.github.io/mapbox-storymap/leaflet-only.html

## MapboxGL and Mapbox.js Dependency
requires a Mapbox account token (free up to 50,000 views per month)

MapboxGL is supported by all modern browsers (Chrome, FFox, Safari) and Internet Explorer 9+

Note: When testing Apple iPad 1st generation with most recent Safari and Chrome available on that device, the code displayed the alert message, "Your browser does not support Mapbox GL".

###About MapboxGL

if MapboxGL is new for you, but you have prior coding experience, read https://www.mapbox.com/help/mapbox-gl-js-fundamentals/
- no distinction between baselayers and overlay layers
- coordinates in lon,lat (like geoJson and xy coords); NOT lat,lng (like Leaflet, Mapbox.js)

## Compare with
- http://jackdougherty.github.io/leaflet-storymap/index.html
- http://jackdougherty.github.io/leaflet-stories/index.html


## Credits
Mapbox GL story map with scroll fly-to https://www.mapbox.com/mapbox-gl-js/example/scroll-fly-to/

Mapbox GL story map (Madrid airport runway) https://www.mapbox.com/bites/00045/

Mapbox storymap tutorial (Sherlock Holmes) (https://www.mapbox.com/mapbox.js/example/v1.0.0/scroll-driven-navigation/

## To Do
- FIX bug in leaflet-only version (using beta 1.x for map.flyTo feature)
- KEY PROBLEM: current version does NOT properly make narrative sections 'active' when scrolling upward. See these console errors:
  - Uncaught TypeError: Cannot read property 'lat' of null
  - setActiveChapter	@	index.html:211
  - window.onscroll	@	index.html:200
- Is this caused by a mismatch when moving from MapboxGL (lng, lat) to Leaflet (lat,lng)?

- add code to automatically resize and center images to fit narrative div width (as in pulse version)
- ask Mapbox support: can Mapbox GL JS  display third-party tileLayers (such as CartoDB LightAll and CT Aerial 1934 WMS) with layer control; start with this example: https://www.mapbox.com/mapbox-gl-js/example/third-party/
- can third-party tileLayers change with narrative sections/chapters?
- can MapboxGL display geojson polygons on specific narrative sections/chapters, to tell stories about boundaries (not just points)?
- ask Mapbox support: when testing IE 8, my browser support code alert did not appear, even though it's based on the same code as this sample that correctly displays, with a reminder to update IE (https://www.mapbox.com/mapbox-gl-js/example/check-for-support/)
