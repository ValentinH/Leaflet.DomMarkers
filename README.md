# Leaflet.DomMarkers
Leaflet Markers with a custom DOM element icon.

Leaflet.DomMarkers.Icon extends the Leaflet.DivIcon object so the same config properties can be used (except the `html` one which is replaced by `element`

The initial idea was to be used inside the [angular-leaflet-directive](https://github.com/tombatossals/angular-leaflet-directive/) and to display interactive icons on the map. The DOM element is generated by the *angular-leaflet-directive* and provided to the Leaflet.DomMarkers.Icon through the `element` property:

```js
var domElement = yourDomElementCreationFunction();
var icon = L.DomMarkers.icon({
  element: domElement,
  iconSize: [20, 20],
  //... other Icon/DivIcon properties
});
```
