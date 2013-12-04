leaflet-zoom-min
===
A Leaflet control that extends `L.Control.Zoom`. It adds a button to the zoom control that allows you to zoom to the map minimum zoom level in a single click.

![Zoom min control screenshot](https://raw.github.com/alanshaw/leaflet-zoom-min/master/screenshot.png)

Usage
---

Add `leaflet-zoom-min` JS and CSS to your page:

```html
<link rel="stylesheet" href="L.Control.ZoomMin.css" media="screen">
<script src="L.Control.ZoomMin.js"></script>
```

Add the zoom min control to your map:

```javascript
var map = L.map("map", {
  layers: L.tileLayer("http://{s}.tile.cloudmade.com/API-key/997/256/{z}/{x}/{y}.png"),
  center: [51.505, -0.09],
  zoom: 3,
  minZoom: 2,
  maxZoom: 16,
  zoomControl: false
})

map.addControl(new L.Control.ZoomMin())
```
